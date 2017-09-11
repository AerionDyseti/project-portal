<template>
  <div class="project-list">
    <div class="row" v-for="project in projects" :key="project.projectName">
        <div class="project-name col-md-5">{{project.projectName}}</div>
        <div class="project-repo col-md-7"><a :href="project.repoUrl">{{project.repoUrl}}</a></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'project-list',
  data () {
    return {
      projects: [
        { projectName: 'Project Portal', repoUrl: 'http://github.com/aeriondyseti/project-portal/' },
        { projectName: 'Resonnace DTMS', repoUrl: 'http://github.com/aeriondyseti/resonance/' },
        { projectName: 'AD House Cup', repoUrl: 'http://github.com/aeriondyseti/housecup/' }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.project-name {
    text-align: right;
}

.project-repo {
    text-align: left;
}

</style>
