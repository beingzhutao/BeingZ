---
layout: default-with-comments
title: "Podcast"
---

## Podcast
*Don’t forget to leave a like and a comment to let me know what you think! 😊*

<br>

<body>
  <ul id="audio-list"></ul>
  <script>
    const dir = "assets/podcast/";
    const audioList = document.getElementById("audio-list");

    fetch(dir)
      .then(response => response.text())
      .then(text => {
        const parser = new DOMParser();
        const html = parser.parseFromString(text, "text/html");
        const links = html.querySelectorAll("a");

        links.forEach(link => {
          const file = link.getAttribute("href");
          if(file.endsWith(".mp3")) {
            const listItem = document.createElement("li");
            const audio = document.createElement("audio");
            const source = document.createElement("source");

            source.src = dir + file;
            source.type = "audio/mpeg";

            audio.appendChild(source);
            audio.controls = true;

            listItem.appendChild(audio);
            audioList.appendChild(listItem);
          }
        });
      })
      .catch(error => console.error(error));
  </script>
</body>