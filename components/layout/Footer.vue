<template>
    <div class="footer mt-5">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <h5>Contato</h5>
            <ul>
              <li>Endereço: Rua Exemplo, 123</li>
              <li>Telefone: (11) 1234-5678</li>
              <li>Email: contato@exemplo.com</li>
            </ul>
          </div>
          <div class="col-md-4">
            <h5>Redes Sociais</h5>
            <ul>
              <li><a href="#">Facebook</a></li>
              <li><a href="#">Twitter</a></li>
              <li><a href="#">Instagram</a></li>
            </ul>
          </div>
          <div class="col-md-4">
            <h5>Sobre Nós</h5>
            <!-- Conteúdo sobre a empresa -->
          </div>
        </div>
  
        <!-- Direitos autorais -->
        <p>&copy; 2023 Meu Site. Todos os direitos reservados.</p>
  
      </div>
    </div>

  
  </template>

  <script>
  export default {
    name: 'Footer'
  }
  </script>
  
  <style scoped>
  /* Estilos do rodapé */
  .footer {
    background-color: #333;
    color: white;
    padding: 20px;
  }
  
  .footer h5 {
    margin-top: 0;
  }
  
  .footer ul {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  
  .footer li {
    margin-bottom:10px;
  }
  
  .footer p {
      text-align:center; 
      margin-top:30px; 
      margin-bottom:0
  }
    
  .footer-links a{
      color:white; 
      text-decoration:none
  }
    
  .footer-links a:hover{
      color:#4180CB; 
      text-decoration:none
  }
    
  .footer-links li{
      display:inline-block; 
      padding-right:20px; 
      padding-left:20px
  }
    
  .footer-links li:last-child{
     padding-right:0
  }
    
  @media (max-width :767px){
     .footer-links li{
         display:block; 
         padding-right:0; 
         padding-left:0; 
         text-align:center
     }
  }
  
  </style>