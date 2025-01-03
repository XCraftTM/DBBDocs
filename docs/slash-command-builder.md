---
hide:
  - toc
icon: material/toolbox
---

<style>
      body {
            overflow: hidden !important;
      }
      .md-grid {
            max-width: 100rem !important;
      }
      .md-main__inner {
            margin-top: 0 !important;
      }
      .md-content__inner:before {
            display: none;
      }
      .md-content__inner {
            padding-top: 0.1px !important;
      }
      @media (max-width: 1219px) {
            .md-sidebar {
                  z-index: 99999999 !important;
            }
            .md-overlay {
                  z-index: 99999999 !important;
            }
      }
      #slash-command-builder {
            display: none;
      }
      .fullScreen {
            width: 100%;
            height: 96%;
            position: absolute;
            top: -100;
            left: 0;
            z-index: 999999;
            pointer-events: auto;
      }
      .notfullscreen {
            height: 850px
      }
      .buttonexit {
            border: "10px";
            color: white;
            padding: 16px 32px;
            top: 100;
            left: 0;
            text-align: center;
            text-decoration: none;
            position: fixed;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            transition-duration: 0.4s;
            cursor: pointer;
            z-index: 9999999 !important;
      }

      .modern-button-exit {
            z-index: 9999999 !important;
            top: 1%;
            left: 46%;
            position: fixed;
      display: inline-block;
      padding: 12px 24px;
      font-size: 16px;
      font-weight: bold;
      text-transform: uppercase;
      text-align: center;
      color: #fff;
      background: linear-gradient(135deg, #e53935, #b71c1c);
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.3s ease-in-out;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .modern-button-exit:hover {
      background: linear-gradient(135deg, #b71c1c, #e53935);
      box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
    }

    .modern-button-exit:active {
      box-shadow: 0 3px 5px rgba(0, 0, 0, 0.2);
    }

      .modern-button {
      display: inline-block;
      padding: 12px 24px;
      font-size: 16px;
      font-weight: bold;
      text-transform: uppercase;
      text-align: center;
      color: #fff;
      background: linear-gradient(135deg, #4caf50, #2e7d32);
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.3s ease-in-out;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .modern-button:hover {
      background: linear-gradient(135deg, #2e7d32, #4caf50);
      box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
    }

    .modern-button:active {
      box-shadow: 0 3px 5px rgba(0, 0, 0, 0.2);
    }
</style>

# :material-toolbox: Slash Command Builder

<iframe id="commandbuilder" class="notfullscreen" src="https://slash.dbb.software/" height="100%" width="100%" frameborder="0" allow="clipboard-write"></iframe>

<button type="button" class="modern-button" id="fsbtn">Enter Fullscreen</button>

<script>
      let fsbtn = document.getElementById("fsbtn");
      fsbtn.onclick = () => {
            let cmdbuilder = document.getElementById('commandbuilder');
            console.log(cmdbuilder.className)
            if(cmdbuilder.className.includes('fullScreen')) {
                  cmdbuilder.className = 'notfullscreen';
                  fsbtn.className = "modern-button"
                  fsbtn.innerHTML = "Enter Fullscreen"
            } else {
                  cmdbuilder.className = 'fullScreen';
                  fsbtn.className = "modern-button-exit"
                  fsbtn.innerHTML = "Exit Fullscreen"
            }
      }
</script>
