<script>
export default {
  created() {
    const { params, query } = this.$route
    const { path } = params
    console.log('path=======', path)
    console.log('query======', query)
    this.$router.replace({ path: '/' + path, query }) // 直接进行重定向
  },
  render: function(h) {
    return h() // avoid warning message
  }
}
</script>
