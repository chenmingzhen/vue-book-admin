<script>
export default {
  name: 'MenuItem',
  functional: true,
  props: {
    icon: {
      type: String,
      default: 'edit'
    },
    title: {
      type: String,
      default: 'world'
    }
  },
  mounted() {
    console.log(this.$route)
  },
  render(h, context) {
    const { icon, title } = context.props
    const vnodes = []
    if (icon) {
      vnodes.push(<div> {(icon)}</div>)
    }

    if (title) {
      vnodes.push(<div> {icon}</div>)
    }
    return vnodes
  }
}
</script>
