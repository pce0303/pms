<script>
  import Project from "./Project.svelte";

  let projects = [{ id: 1, name: '첫 번째 프로젝트' },
  { id: 2, name: '두 번째 프로젝트' },
  { id: 3, name: '세 번째 프로젝트' },
  { id: 4, name: '네 번째 프로젝트' },
  { id: 5, name: '다섯 번째 프로젝트' },
  { id: 6, name: '여섯 번째 프로젝트' },
  { id: 7, name: '일곱 번째 프로젝트' },
  { id: 8, name: '여덟 번째 프로젝트' },
  ]
</script>

  <h2><b>My Projects</b></h2>
  <div class="project-container">
    <ul>
      {#each projects as project}
        <li>
          {project.id}
          {project.name}
        </li>
      {/each}
    </ul>
  </div>
  <p class="index"><b>1</b> 2 3 next</p>

<style>
  .project-container {
    
  }
  
  li {
    margin: 1em;
    padding: 10px;
    list-style: none;
    border-radius: 10px;
    background-color: white;
  }

  .index {
    display: block;
    align-self: center;
  }
</style>