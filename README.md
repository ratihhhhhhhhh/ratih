<div id='content'> halo </div>

<script>


  pbo={
  model:{
  mahasiswa:[
    {username:'ratih',pin:'ratih123'},
    {username:'afwanda',pin:'afwanda123'},
    {username:'shandy',pin:'sandi123'},
  ],
  },
  services:{
    getter:function(){ alert('getter')},
    setter:function(){ alert('setter')},
  },
  view:{
    signform:function(arr){
  return `
  username <input type='txt' value='' id='username'><br/>
  pin <input type='password' value='' pin='pin'><br/>
  <button id='login' > Login </button><br/>
  <button id='cancel' >cancel </button><br/>
  `;
    },
  },
  controller:{
    signin:function(){ document.getElementById('id').onclick=function(){alert('login')}},
    signout:function(){
      document.getElementById('username').value='';
      document.getElementById('pin').value='';
  },
    signform:function(){
      document.getElementById('content').innerHTML=model.view.signform('arr');
      document.getElementById('pin').value='';
  },
    

  },

  }


pbo.controller.signform();

 </script>
