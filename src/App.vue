<!-- 
<template>
  <div>
    <h1>{{parseInt(num)+parseInt(num2==0?1:num2) }}</h1>
    <input type="text" placeholder="telefono" v-model.trim="num">
    <input type="text" placeholder="telefono" v-model="num2">
  </div>
</template>

<script setup>
import {ref} from "vue"
  let num=ref(0)
  let num2=ref(0)
let telefono =ref(38494949)
telefono.value="777"
let nombre=ref("contreras")
nombre.value =telefono.value
</script> -->


<!-- <template>
  <div>
<h1>{{lenguaje}}</h1>
  <input type="radio" v-model="lenguaje" value="java" ><label for="interesado">java</label> 
  <input type="radio" v-model="lenguaje" value="javascript" ><label for="javascritp">javascript</label>


<h1>{{idioma}}</h1>
<select v-model="idioma">
<option value="python">python</option>
<option value="java">java</option>
<option value="javascript">javascript</option>
<option value="php">php</option>
</select>

  </div>
</template>

<script setup>
import {ref} from "vue"
  let lenguaje=ref("")
  let idioma=ref("")

</script> -->


<!-- <template>
  <div>
<h1>{{contador}}</h1>
<button @click="contar()">cambiar</button>  
<h2 v-if="contador<21">hol SOY EL MSJ Q VAN A DESAPARECER</h2>
<h2 v-else>hol SOY EL MSJ Q VAN A DESAPARECER</h2>

<h2>{{contador<21?"hola soy el ..":"hola soy otro"}}</h2>
  </div>
</template>

<script setup>
import {ref} from "vue"
  let contador=ref(0)
function contar(){
  contador.value+=1
}
</script> -->

<!-- 
<template>
  <div>

    <h1>{{operacion}}</h1>

    <input type="text" placeholder="num1" v-model.trim="num">
    <input type="text" placeholder="num2" v-model="num2">

  <input type="radio" v-model="ope" value="suma" ><label for="suma">suma</label> 
  <input type="radio" v-model="ope" value="resta" ><label for="resta">resta</label>
  <input type="radio" v-model="ope" value="multiplicacion" ><label for="multiplicacion">multiplicacion</label>
  <input type="radio" v-model="ope" value="division" ><label for="division">division</label>

  <button @click="contar()">operar</button>  

  </div>
</template>

<script setup>
import {ref} from "vue"

  let num=ref(0)
  let num2=ref(0)
  let operacion=ref(0)
  let ope=ref("")

function contar(){
  if(ope.value=="suma"){
operacion.value=parseIntnum.value+parseIntnum2.value
  }else if(ope.value=="resta"){
operacion.value=parseIntnum.value-parseIntnum2.value 
  }else if(ope.value=="multiplicacion"){
operacion.value=parseIntnum.value*parseIntnum2.value
} else if(ope.value=="division" && num2.value==0?1:(num2.value)){
operacion.value=parseIntnum.value/parseIntnum2.value}
}

</script>  -->


 <!-- <h3 :style="alerta==='Formulario enviado correctamente'?'color:green':''">{{ alerta }}</h3>
    <h1>Formulario</h1>
    <form>
      <label for="nombre">Nombre:</label>
      <input type="text" id="nombre" name="nombre" v-model="nombre">
      <label for="apellidos">Apellidos:</label>
      <input type="text" id="apellidos" name="apellidos" v-model="apellidos">
      <label for="tipo_documento">Tipo documento:</label>
      <select id="tipo_documento" name="tipo_documento" v-model="tipo_documento">
        <option value="cedula">Cédula</option>
        <option value="tarjeta_identidad">Tarjeta de identidad</option>
        <option value="pasaporte">Pasaporte</option>
      </select>
      <label for="numero_documento">Número de documento:</label>
      <input type="text" id="numero_documento" name="numero_documento" v-model="numero_documento">
      <label for="genero">Genero:</label>
      <select id="genero" name="genero" v-model="genero">
        <option value="masculino">Masculino</option>
        <option value="femenino">Femenino</option>
        <option value="otro">Otro</option>
      </select>
      <label for="correo">Correo:</label>
      <input type="email" id="correo" name="correo" v-model="correo">
      <label for="telefono">Teléfono:</label>
      <input type="text" id="telefono" name="telefono" v-model="telefono">
      <label for="fecha_nacimiento">Fecha de nacimiento:</label>
      <input type="date" id="fecha_nacimiento" name="fecha_nacimiento" v-model="fecha_nacimiento">
      <label for="telefono">Edad:</label>
      <input type="number" id="telefono" name="telefono" v-model="edad1">
    </form>
    <button @click="validar()">enviar</button>

    <table>
      <thead>
        <tr>
          <th>Nombre</th>
          <th>Apellido</th>
          <th>Tipo de documento</th>
          <th>Numero de documento</th>
          <th>Telefono</th>
          <th>Correo</th>
          <th>Genero</th>
          <th>Fecha de nacimiento</th>
          <th>edad</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, i) in registros" :key="i" :style="item.edad>17?'color:pink':'color:purple'">
          <td>{{ item.nombre }}</td>
          <td>{{ item.apellidos }}</td>
          <td>{{ item.tipo_documento }}</td>
          <td>{{ item.numero_documento }}</td>
          <td>{{ item.telefono }}</td>
          <td>{{ item.correo }}</td>
          <td>{{ item.genero }}</td>
          <td>{{ item.fecha_nacimiento }}</td>
          <td>{{ item.edad }}</td>
        </tr>

      </tbody>

    </table>  -->

    <!-- <img :src="image" alt="" :style="{borderRadius:num}"> -->
    <!-- <h1 :style="{borderRadius:12}">hola a todos</h1> -->
    <!-- <h1 :style="num>18?'color:salmon':'color:green'">mi edad es {{ num }}</h1> -->

  <!-- </div>
</template> -->

<!-- 
<script setup>
import {ref} from "vue"
let num = ref(19)
let color = ref("yellow")
let image = ref("https://adrianalonso.es/wp-content/uploads/2018/01/vue.jpg") -->


<!-- 
<template>
  <div>
<div id="todo">


<textarea id="alert" v-if="alerta" v-model="alerta"> </textarea>
<button @click="closealert()" v-show="alerta">cerrar</button>

<div id="inicio">
    <label for="nombre">Nombre</label> <input type="text" placeholder="nombre" v-model.trim="nombre">
    <label for="apellido">Apellido</label> <input type="text" placeholder="apellido" v-model.trim="apellido">
<div id="sele">
      <label for="opciones">Tipo de documento</label>
      <select v-model="Tipodocumento">
        <option disabled selected="">selecciona un tipo de documento</option>
          <option value="ti">Tarjeta de identidad</option>
          <option value="Cedula">Cédula</option>
          <option value="extranjera">Extranjera</option>
      </select>
 </div>
    <label for="documento">Documento</label> <input type="text" placeholder="n.documento" v-model.trim="documento">
    <label for="sexo">Correo:</label> <input type="email" placeholder="Escriba su email" v-model.trim="email">
    <label for="fecha">Fecha de nacimiento:</label><input type="date" v-model="fecha">
    <label for="doc">Numero de telefono:</label><input type="tel" placeholder="N. de telefono" v-model="telefono">
</div>

<div id="sex">
  <input type="radio" v-model="gen" value="masculino" ><label for="masculino">masculino</label> 
  <input type="radio" v-model="gen" value="femenino" ><label for="femenino">femenino</label>
</div>


  <button id="regi" @click="validar()">Registrar</button>  

</div>
<table>
      <thead>
        <tr>
          <th>Nombre</th>
          <th>Apellido</th>
          <th>Tipodocumento</th>
          <th>documento</th>
          <th>telefono</th>
          <th>email</th>
          <th>gen</th>
          <th>fecha</th>
          <th>Opciones</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, i) in registros" :key="i" :style="item.edad>17?'color:pink':'color:purple'">
          <td>{{ item.nombre }}</td>
          <td>{{ item.apellido }}</td>
          <td>{{ item.Tipodocumento }}</td>
          <td>{{ item.documento }}</td>
          <td>{{ item.telefono }}</td>
          <td>{{ item.email }}</td>
          <td>{{ item.gen }}</td>
          <td>{{ item.fecha }}</td>
          <td>
            <button @click="eliminar(i)">❌</button>
            <button @click="editar(item, i)">📝</button>
          </td>
        </tr>

      </tbody>

    </table> 
  </div>
</template>


<script setup>
import {ref} from "vue"


function closealert() {
  alerta.value=""
  }

let registros = ref([]);
let nombre=ref("")
let apellido=ref("")
let Tipodocumento=ref("")
let documento=ref("")
let email=ref("")
let fecha=ref("")
let telefono=ref("")
let gen=ref("")
let alerta=ref("")
let bd=true
let index=null

function eliminar(i){
  registros.value.splice(i,1)
}

function editar(item, i){
  console.log(item);
  console.log(i);
  nombre.value = item.nombre
  apellido.value = item.apellido
  gen.value = item.gen
  email.value = item.email
  fecha.value = item.fecha
  Tipodocumento.value = item.Tipodocumento
  documento.value = item.documento
  telefono.value = item.telefono
bd=false
index=i

}

function validar(){
        
  let vericorreo = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;
if (bd==true){

  if(nombre.value==""){
  alerta.value= "Por favor seleccione su nombre"
  }else if(apellido.value==""){
    alerta.value="Por favor digite su apellido"
  }else if(Tipodocumento.value==""){
    alerta.value="Por favor seleccione un Tipo de documento"
  } else if(documento.value.length<6){
    alerta.value="Por favor su documento debe tener mas de 7 digitos"
  }else if(!vericorreo.test(email.value)){
    alerta.value="Por favor escriba su correo"
  }else if(fecha.value==""){
    alerta.value="Por favor escriba su fecha"
  }else if(((new Date().getFullYear() - new Date(fecha.value).getFullYear))<18){
    alerta.value="debe ser mayor de edad"
  }else if(telefono.value.length<10){
    alerta.value="Por favor digite su telefono con mas de 10 digitos"
  }else if(gen.value==""){
  alerta.value="Por favor seleccione un genero"
    } 
    else
   alerta.value = "Formulario enviado correctamente";
          registros.value.push({
    nombre: nombre.value,
    apellido: apellido.value,
    gen: gen.value,
    email: email.value,
    fecha: fecha.value,
    Tipodocumento: Tipodocumento.value,
    documento: documento.value,
    telefono: telefono.value
          })
  console.log(registros);
}
else{
  registros.value[index].nombre=nombre.value
  registros.value[index].apellido=apellido.value
  registros.value[index].gen=gen.value
  registros.value[index].email=email.value
  registros.value[index].fecha=fecha.value
  registros.value[index].Tipodocumento=Tipodocumento.value
  registros.value[index].documento=documento.value
  registros.value[index].telefono=telefono.value

  bd=true
}

}



</script>


<style scoped>

#todo{
  width:60vw;
  height:50vh;
  margin:2px solid black;
display:grid;
}
#inicio{
  display: grid;
    width:40%;
  height:40vh;
  margin:2px solid white;

}
#sex{
display:flex
}
#regi{
  width:20%;
  height:5vh;
}
#alert{
  height:3vh;
  width:41%;
}

th, tr, td{
  border: 2px solid blue;
}

form {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  width: 80%;
  height: 60vh;
  margin-bottom: 20px;
  background-color: #5a007d;
  padding: 10px;
}

input{
  width: 100%;
}

select {
  width: 100%;
  padding: 2px;
} 

</style> -->


<template>
    <div id="inicio">
    <div id="alert">
    <textarea  v-if="alerta" v-model="alerta"> </textarea>
<button @click="closealert()" v-show="alerta">cerrar</button>
</div>
    <div id=actividad>
    <label for="actividad">Actividad</label> <input id="act" type="text" v-model.trim="actividad">
    <label for="prioridad">Prioridad Alta</label > <input id="bot" type="checkbox" v-model="prioridad" >
    <label for="fecha">Fecha</label > <input id="pri" type="date" placeholder="fecha" v-model="fecha">
    </div>
    <div id="botones">
    <button @click="generar()">+</button> 
    </div>
    <div id="botones">
    <button @click="ordenar()">Ordenar</button> 
    </div>

<div id="tabla">
    <table>
      <thead>
        <tr>
          <th>ACTIVIDAD</th>
          <th>PRIORIDAD</th>
          <th>FECHA</th>
          
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, i) in activi" :key="i" :style="item.prio==='alta'?'color:red':'color:white'">
          <td>{{ item.actividad }}</td>
          <td>{{ item.prio }}</td>
          <td>{{ item.fecha }}</td>
          <td> <button @click="eliminar(i)">❌</button></td>
        </tr>
      </tbody>
    </table>
    </div>
      </div>

</template>


<script setup>
import {ref}from "vue" 
  
function closealert() {
  alerta.value=""
  }
let actividad=ref("")
let activi=ref([])
let fecha=ref("")
let prioridad=false
let prio=""
let alerta=ref("")


function generar(){

  if (prioridad==true){
    prio="alta"
  }else prio="baja"
 activi.value.push({
  actividad: actividad.value,
  fecha: fecha.value,
  prio: prio
   })       
if(actividad.value==""){
alerta.value= "Por favor escriba su actividad"
}else if(fecha.value==""){
  alerta.value="Por favor escriba su fecha"
  } 
console.log(activi.value)
}

function ordenar(){
return activi.value.sort((a,b)=>{
  if(a.prio==="alta")return -1;
  if(b.prio==="alta")return 1;
  return 0;
})
}

function eliminar(i){
  activi.value.splice(i,1)
}

</script>


<style coped>

#actividad{
display:flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
gap:2%;
   width:30vw;
    height:24vh;
    color:white;
    font-weight: 500;
}
#alert{
  position: absolute;
  width:17vw;
  height:8vh;
}
textarea{
  background:rgb(206, 65, 65);
  padding: 4%;
  font-size: large;
}
#inicio{
  display:flex;
  flex-direction: column;
  gap:4%;
  justify-content: center;
  align-items: center;
   width:40vw;
    height:65vh;
}

#priori{
  width:30px;
  height:20px;
}
#bot{
  width:2vw;
  height: 5vh;
}
#act{
  width:80%;
  font-size: large;
    height:4vh;
}

#pri{
    width:10vw;
    height:3vh;
}

table{
    width:25vw;
    height:20vh;

}
#tabla{
    overflow:scroll;
}

#botones{
    width:9vw;
    height:6vh;
}
</style>
