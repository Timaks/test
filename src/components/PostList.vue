<template>
<div>
    <h3>Список пользователей</h3>
      <post-item v-for="post in posts" 
      :post="post"
      :key="post.id"
      @remove="$emit('remove', post)"
      />
</div>
</template>

<script>
import PostItem from './PostItem';
export default {
    components: {PostItem},
    //пропсы изменять нельзя
    props: {
        posts: {
            type: Array,
            required: true,
        }
    }
}
</script>

<style scoped>

</style>