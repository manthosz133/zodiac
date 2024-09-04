<template lang="">
    <div className="card">
      <!-- <img src="https://img.freepik.com/premium-vector/vector-childrens-strange-adventures_1103584-155.jpg" alt="Avatar" style="width:100%">
        <div class="container">
          <h4><b>John Doe</b></h4> 
          <p>Architect & Engineer</p> 
        </div>

      <img src="https://img.freepik.com/premium-vector/vector-childrens-strange-adventures_1103584-155.jpg" alt="Avatar" style="width:100%">
        <div class="container">
          <h4><b>view</b></h4> 
          <p>Atmosphere pictures</p> 
        </div>

        <img src="https://img.freepik.com/premium-photo/free-beautiful-green-garden-cartoon-background-illustration-generative-ai_627719-5536.jpg" alt="Avatar" style="width:100%">
        <div class="container">
          <h4><b>John Doe</b></h4> 
          <p>Architect & Engineer</p> 
        </div> -->

<img :src="image" alt="name" style="width:100%">
      <div class="container">
        <h4> <b> {{name}} </b></h4>
        <p>{{nickname}}</p>
        <p>{{text}}</p>
      </div>
    </div>
</template>

<script>
export default {
    props: ['id','name','nickname','text','image']
}
</script>
<style scoped>
    /* .card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 40%;
} */

.card {
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
  transition: 0.3s;
  border-radius: 10px;
  overflow: hidden;
  background-color: rgba(255, 255, 255, 0.9); /* สีขาวโปร่งแสง */
}

.card:hover {
  box-shadow: 0 8px 16px rgba(0,0,0,0.3);
}

.card-image {
  width: 100%;
  height: auto;
}

.card-content {
  padding: 16px;
}

.card-content h4 {
  margin: 0;
  font-size: 1.2rem;
}

.nickname {
  font-style: italic;
  color: #555;
}

.description {
  color: #777;
  margin-top: 8px;
}


</style>