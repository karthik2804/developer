<script>
import ContentFilter from './ContentFilter.vue'
import ContentListing from './ContentListing.vue'
export default {
    components: { ContentFilter, ContentListing }
}
</script>

<template>
    <div class="content-wrapper">
        <div class="columns content-inner is-0 is-mobile is-multiline">
            <ContentFilter />
            <ContentListing />
        </div>
    </div>
</template>

<style lang="scss" scoped>
.content-wrapper {
    width: 100%;
    display: flex;
    margin-top: 2rem;
    border-top: 1px solid rgba($lavender, 0.333);
    background: linear-gradient(180deg,
        rgba(230, 210, 241, 0.05) 0%,
        rgba(230, 210, 241, 0.00) 100%
    );
}

@media screen and (max-width:1023px) {
    // .content-wrapper {
    //     flex-direction: column;
    // }
}
</style>