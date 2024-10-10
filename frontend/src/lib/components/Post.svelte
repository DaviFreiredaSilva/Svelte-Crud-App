<script>
  export let post
</script>

<div class="card text-dark w-75 mb-4">
    <div class="card-header">{post.created_at}</div>
    <div class="card-body">
      <h5 class="card-title">{post.title}</h5>
      <a href="/{post.post_id}" class="btn btn-primary">Click to read</a>
    </div>
  </div>