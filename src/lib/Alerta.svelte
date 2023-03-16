<script>
   import * as bootstrap from 'bootstrap'


    let bsAlert;
    const setAlert=(div)=>{
        bsAlert = new bootstrap.Alert(div)
        console.log(bsAlert);
    }

    const cerrarAlerta=()=>{
        bsAlert&&bsAlert.close();
    }
</script>


<div class="alert alert-primary" role="alert" use:setAlert>
    A simple primary alert—check it out!
  </div>

  <button class="btn" on:click|once={cerrarAlerta}>Cerrar</button>