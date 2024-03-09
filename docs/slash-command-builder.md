icon: material/toolbox

# :material-toolbox: Slash Command Builder

<iframe id="commandbuilder" src="https://beastlybear2017.github.io/Discord-Slash-Command-Builder/" height="269px" width="100%" frameborder="0" scrolling="no" allow="clipboard-write"></iframe>

---

This is a Slash Command Builder that was originally created by [Sebastian on Github](https://github.com/bsati/dc-app-command-builder), and has since been updated by BeastlyBear2017, with a link to the hosted website [here](https://beastlybear2017.github.io/Discord-Slash-Command-Builder/).


<script>
      // https://beastlybear2017.github.io/Discord-Slash-Command-Builder/
      // http://localhost:8080
      const iframe = document.getElementById('commandbuilder')
      window.addEventListener('message', message => {
      if (message.source !== iframe.contentWindow) return
            iframe.height = message.data.msg
      }, false);
</script>