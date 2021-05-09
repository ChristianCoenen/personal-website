<script>
  import Entry from "./Entry.svelte";
  export let name;

  const items = [];

  items.push({
    label: "Intro",
    content: [
      {
        header: "Introduction",
        body:
          "<b>Hey, I'm Chris.</b> I love to <pre style='display:inline;font-size:16px'>CODE</pre> and to solve problems. |I work best in open, creative and supportive environments. |If you scroll down the Timeline, you can find a history of some projects I'm particularly proud of 😊.||{0}|{1}",
        list: [],
        links: [
          { href: "https://www.github.com/ChristianCoenen", desc: "Github" },
          { href: "mailto:coenen.christian@outlook.com", desc: "Reach out" },
        ],
      },
    ],
  });

  items.push({
    label: "Ongoing",
    content: [
      {
        header: "Content Creation on YouTube",
        body:
          "{0} |TODO: write description here",
        list: [],
        links: [
          {
            href: "https://www.youtube.com/BotAcademyYT",
            desc: "Channel Link",
          },
          { href: "https://www.ptc.com/", desc: "PTC" },
        ],
        image: "botacademy.png"
      },
    ],
  });

  items.push({
    label: "2021",
    content: [
      {
        header: "Masters degree at University of Applied Sciences Mannheim ✅",
        body: "Courses:",
        list: [
          "TODO",
        ],
      },
      {
        header: "Automated Content Creation",
        body: "TODO: describe project",
        list: [
          "TODO",
        ],
      },
    ],
  });
</script>

<style>
  :global(body) {
    --accent: #ffca28;
    --background: #253136;
    --borders: #add8e636;
    width: 1000px;
    max-width: 98vw;
    margin: auto;
    height: auto;
    color: white;
    padding: 0;
    padding-bottom: 50px;
    background: linear-gradient(to left, black 5%, var(--background));
    background-size: 100%;
    background-repeat: no-repeat;
  }

  @media (prefers-color-scheme: light) {
    :global(body) {
      --accent: #61c89d;
      --background: #f9f9f9;
      --borders: #00000052;
      color: #292929;
    }
    :global(a) {
      font-weight: 500;
    }
  }

  :global(body:before) {
    content: "";
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    width: 100%;
    z-index: -1;
    background: var(--background);
  }

  h1 {
    text-align: center;
    margin-bottom: 50px;
    padding-top: 150px;
  }

  .spacer {
    padding-left: 25px;
    border-left: 2px solid var(--accent);
    margin-left: 25px;
    width: 100%;
    background: linear-gradient(
      to right,
      transparent 5%,
      rgba(255, 255, 255, 0.05) 95%
    );
    min-height: calc(360px - 35vw);
  }

  .item {
    display: flex;
    position: relative;
  }

  .label::after {
    content: "";
    position: absolute;
    right: -31px;
    top: 6px;
    background: var(--accent);
    height: 10px;
    width: 10px;
  }

  .label {
    flex: 1 1 17%;
    margin-left: 4%;
    margin-bottom: 25px;
    margin-top: 23px;
    top: 22px;
    max-width: 17%;
    text-align: center;
    display: inline-table;
    position: sticky;
    word-break: break-word;
  }

  @media (max-width: 600px) {
    .label {
      flex: 1 1 10px;
      width: 10px;
      min-width: 10px;
      max-width: 10px;
    }
  }
</style>

<h1>My Timeline</h1>

{#each items as year}
  <div class="item">
    <div class="label">{year.label}</div>
    <div class="spacer">
      {#each year.content as item}
        <Entry config={item} />
      {/each}
    </div>
  </div>
{/each}
