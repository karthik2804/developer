<script>
import HubIntro from './components/HubIntro.vue'
import ContentSpace from './components/ContentSpace.vue'
import PreviewModal from './components/PreviewModal.vue'

export default {
    components: {HubIntro, ContentSpace, PreviewModal},
}
</script>

<template>
    <div class="main hub" >
        <HubIntro/>
        <ContentSpace />
        <PreviewModal />
    </div>
</template>

<style lang="scss">
body {
    width: 100%;

    &.modal-open {
        height: 100%;
        overflow: hidden;
    }
}

.main {
    width: 100%;
    overflow: hidden;
    min-height: 100vh;
}

.columns {
    max-width: 88rem;
    margin-left: auto;
    margin-right: auto;
}
</style>
