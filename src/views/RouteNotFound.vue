<script>
import router from "../router";

const vue = {
  name: "route-not-found",

  // redirect to Banana Mirror Browser, since this is the only page on that website
  mounted: function () {
    router.push("/celeste/banana-mirror-browser");
  },
};

export default vue;
</script>
