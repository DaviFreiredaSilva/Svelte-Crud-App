<script>
    import {postStore} from '../../store.js'
    export let data;

    let post=$postStore.find((p)=> p.post_id == data.id)

</script>

<div class="card text-dark w-75 mb-4">
    <div class="card-header fs-3 fw-bold text-capitalize">{post.title}</div>
    <div class="card-body">
        <p>Author: {post.author}</p>
      <h5>{post.content}</h5>
      <p class="card-title">Tags: {post.tags}, Created at {post.created_at}</p>
      <p>{post.views} views</p>
      <a href="/" class="btn btn-primary my-3">Back to Home</a>
    </div>
</div>