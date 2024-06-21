<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>Roberto Ezequiel Chacón Rosales.</p>
    <p>Backend</p>

    <h3>Enlaces a Páginas</h3>
    <div class="button-container">
      <button @click="scrollToSection('about')">Acerca de</button>
      <button @click="scrollToSection('skills')">Habilidades</button>
      <a href="https://github.com/chacon503" target="_blank" class="button">Proyectos</a>
    </div>

    <div id="about" class="section">
      <h2>Acerca de</h2>
      <p>Soy un estudiante de ingeniería en sistemas de la Universidad Adventista de Centro América, 
        tengo una pasión por aprender y adquirir habilidades nuevas.
        <br><br>
        En lo poco que llevo estudiando mi carrera universitaria, he aprendido a resolver problemas 
        complejos, y hacer que las cosas funcionen de la mejor manera. 
        Tengo conocimientos previos en programación, telemática y redes, también en base de datos, y sistemas operativos. 
        <br><br>
        Unas de las ramas de esta ingeniería que me gustan son las siguientes: ciber seguridad, telemática y redes. 
        Cuando finalice mi carrera, pretendo especializarme en redes y ciber seguridad. Creo que esta especialización me 
        permitirá profundizar en mis conocimientos y habilidades en esta área. Sin embargo, no me he limitado a los cursos 
        de mis materias. He tomado cursos adicionales en programación y sistemas operativos para fortalecer aún más mis
        habilidades y me han proporcionado una comprensión más profunda de estos campos.
        <br><br>
        Estoy emocionado por el camino que tengo por delante. La ingeniería en sistemas es un campo en constante evolución, 
        y estoy ansioso por continuar aprendiendo y creciendo en mi carrera. Cada nuevo concepto que aprendo y cada habilidad 
        que adquiero me acerca un paso más a mi objetivo de convertirme en un ingeniero competente y productivo.
      </p>
    </div>

    <div id="skills" class="section">
      <h2>Habilidades</h2>
      <ul class="skills-list">
        <li>Sistemas Operativos:
          <br>
          Familiaridad con Windows y Linux.
          <br>
          Familiaridad en la administración de servidores.
          <br>
          Redes y Seguridad:
          <br>
          Conocimiento en configuración y administración de redes.
          <br>
          Principios básicos de seguridad informática.
          <br>
          Desarrollo de Aplicaciones Móviles:
          <br>
          Principios básicos de aplicaciones para Android.
          <br>
          Uso de herramientas como Android Studio.
          <br>
          Trabajo en Equipo:
          <br>
          Habilidad para colaborar con equipos.
          <br>
          Comunicación efectiva dentro de un equipo.
          <br>
          Gestión del Tiempo:
          <br>
          Adaptabilidad:
          <br>
          Facilidad para aprender nuevas tecnologías y adaptarse a cambios.
        </li>
        <br>
        <br>
        <br>
        <li>Python</li>
        <li>C#</li>
        <li>Virtualización</li>
        <li>Vue.js</li>
        <li>SQL</li>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>

      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
    scrollToSection(sectionId) {
      const section = document.getElementById(sectionId);
      if (section) {
        section.scrollIntoView({ behavior: 'smooth' });
      }
    }
  }
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
  font-size: 18px;
}

.button-container {
  display: flex;
  justify-content: center;
  gap: 10px;
  margin-top: 20px;
}

button, .button {
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease;
  text-decoration: none;
  color: inherit;
  border: none;
  background-color: #f0f0f0;
}

button:hover, .button:hover {
  background-color: #0000ff;
  color: white;
}

.section {
  margin-top: 20px;
  color: white;
}

.skills-list {
  list-style-type: none; /* Elimina los puntos de la lista */
  padding-left: 0; /* Elimina el espacio izquierdo predeterminado */
}

.skills-list li {
  font-size: 18px; /* Tamaño de letra para las habilidades */
  line-height: 1.6; /* Espaciado entre líneas */
}

#about {
  margin: 150px;
}

#skills {
  margin: 150px;
}

h2 {
  font-size: 24px;
}

p {
  font-size: 18px;
  line-height: 1.6;
}
</style>
