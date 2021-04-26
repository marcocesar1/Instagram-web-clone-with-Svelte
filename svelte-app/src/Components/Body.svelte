<script>
    import Stories from '../Components/Stories.svelte';
    import Suggestions from '../Components/Suggestions.svelte';
    import Post from '../Components/Post.svelte';
</script>

<div class="container">
    <div class="row">
        <div class="col-md-12 col-lg-8 mt-0 mt-sm-4 mb-4">
            <Stories/>
            <Post/>
        </div>
        <div class="col-md-4 mt-4">
            <Suggestions/>
        </div>
    </div>
</div>

<style type="text/scss">
    
</style>