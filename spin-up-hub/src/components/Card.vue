<script>
export default {
    data() {
        return {

        }
    },
    methods: {
        OpenItem() {
            this.$store.dispatch("openPreview", this.$props.item)
        }
    },
    props: ["item"]
}
</script>

<template>
    <div class="column is-one-third" @click="OpenItem">
        <a class="card">
            <header>
                <span class="category">{{ item.category }}</span>
                <span class="icon"></span>
            </header>
            <article>
                {{ item.title }}

                <div class="tags">
                    <span v-for="tag in item.tags">
                        {{ tag }}
                    </span>
                </div>
            </article>
        </a>
    </div>
</template>

<style lang="scss" scoped>
.card {
    margin-bottom: 1rem;
    min-height: 200px;
    display: flex;
    flex-direction: column;
    background: desaturate(darken(rgba($lavender, 0.33), 42.5%), 25%);
    // padding: 1rem;
    border-radius: 1rem;
    transition: all 1s ease-in-out;
    overflow: hidden;

    header {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .category {
            background-color: $lightlavender;
            display: inline-block;
            border-radius: 0.67rem;
            padding: 0.2rem 0.4rem;
            color: $darkspace;
            font-size: 0.8rem;
        }

        .icon {
            width: 20px;
            height: 20px;

            path {
                stroke: black;
            }
        }
    }

    article {
        margin-top: 1rem;
        flex-grow: 1;
        font-size: 1.125rem;
        font-weight: 600;
    }

    .tags {
        font-size: 0.8rem;

        span {
            padding: 0.2rem;
        }
    }
}
</style>