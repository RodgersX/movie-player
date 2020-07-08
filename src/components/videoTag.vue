<template>
    <div class="video-tag">
        <iframe
        allowfullscreen
        frameborder="0"
        height="376"
        :src="source.trailer"
        style="width: 100%; min-width: 750px"></iframe>
    </div>
</template>

<script>
export default {
    props: ['source']
}
</script>