<template>
  <h1>
    Single user dynamic route. Starting file name with _ <br />
    id:{{ $route.params.id }}
  </h1>
</template>

<script>
export default {
  layout: "users",
  validate(data) {
    // console.log(data);
    //regex to validate dynamic segment (id) as a number
    return /^\d+$/.test(data.params.id);
  },
};
</script>
