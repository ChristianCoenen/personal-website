<script>
  import Entry from "./Entry.svelte";
  export let name;

  const items = [];

  items.push({
    label: "Intro",
    content: [
      {
        header: "Introduction 👋",
        body:
                "<b>Hey, I'm Chris.</b> I love to <pre style='display:inline;font-size:16px'>CODE</pre> " +
                "and to solve problems. |I work best in open, creative and supportive environments. " +
                "|If you scroll down the timeline, you can find a history of some projects and achievements " +
                "I'm particularly proud of 😊.||{0}|{1}",
        list: [],
        links: [
          { href: "https://www.github.com/ChristianCoenen", desc: "Github" },
          { href: "https://www.linkedin.com/in/christian-coenen/detail/contact-info/", desc: "Reach out" },
        ],
        image: "me.png"
      },
    ],
  });

  items.push({
    label: "Ongoing",
    content: [
      {
        header: "Content Creation on YouTube 👨🏻‍💻",
        body:
                "During the end of 2019, my desire to create something that helps people is some way grew " +
                "significantly. So I decided to create {0}, a YouTube channel with a focus on " +
                "Automation & Machine Learning." +
                "||Since then, I have created and uploaded multiple videos with a combined view-count of over 130k+." +
                "|I am very happy that my videos seem to provide value to many people every day." +
                "||The source code for projects that I present on YouTube can be found {1}",
        list: [],
        links: [
          {
            href: "https://www.youtube.com/BotAcademyYT",
            desc: "BotAcademy",
          },
          {
            href: "https://github.com/Bot-Academy",
            desc: "here",
          },
        ],
        image: "botacademy.png"
      },
    ],
  });

  items.push({
    label: "2021",
    content: [
      {
        header: "A fully automated YouTube Channel?! 🧑🏻‍💻",
        body:
                "In 2020, two fellow students and I decided to create a fully autonomous YouTube channel. " +
                "||To achieve this, we wrote a program that created gaming compilations from clipped Twitch scenes " +
                "for a given game. Because many of those clips were not ingame clips, we created a neural network " +
                "with the ability to filter them out. Then we wrote a program that publishes " +
                "a given video to our YouTube channel. Finally, we deployed everything on AWS to achieve " +
                "full automation and let it run for 100 days." +
                "||In 2021, after the experiment was over, we documented everything properly, published the {2} " +
                "and posted about it on {0}, where the {1} got over 1000 upvotes. At the time of writing (May 2021), " +
                "the repositories received over 200 ⭐ on GitHub." +
                "||So what did we achieve?",
        list: [
          "We automatically uploaded > 100 videos to {3} without any human interaction",
          "One video got quite some traction by getting 2155 views and 48 likes",
          "All our uploads combined got over 10k views",
          "We didn't receive a single comment indicating the use of bots",
        ],
        links: [
          {
            href: "https://www.reddit.com/r/Python/",
            desc: "r/Python",
          },
          {
            href: "https://www.reddit.com/r/Python/comments/msskzd/code_release_we_created_a_fully_autonomous/",
            desc: "post",
          },
          {
            href: "https://github.com/ContentAutomation",
            desc: "code repositories on GitHub",
          },
          {
            href: "https://www.youtube.com/channel/UCqq27nknJ3fe5IvrAbfuEwQ",
            desc: "our YouTube channel",
          },
        ],
        image: "contentautomation.png"
      },
      {
        header: "Master's degree in Computer Science 🎓",
        body:
                "In February 2021, I graduated from the University of Applied Sciences in Mannheim " +
                "(master, GPA: 3.9)." +
                "||Thesis (incl. source code): {0}" +
                "||Courses:",
        links: [
          {
            href: "https://github.com/ChristianCoenen/Master-Thesis",
            desc: "<i> A new Adversarial Approach for Model Generation " +
                    "in both a Supervised and Reinforcement Learning Context</i>",
          },
        ],
        list: [
          "Neural Networks",
          "Autonomous Mobile Robots",
          "Image Processing",
          "Knowledge Discovery and Management",
          "Container Technology",
          "Compilers",
          "Mobile Software Engineering",
          "Software Development Processes",
          "Software Quality Management",
          "Software Engineering Project",
          "Advanced Research Methods",
          "Computer Science Workshop",
        ],
      },
    ],
  });

  items.push({
    label: "2020",
    content: [
      {
        header: "Cambridge English C1 Advanced Certificate 📜",
        body:
                "On 24. January 2020, I was issued the Cambridge English C1 Advanced Certificate after " +
                "being examined a month prior to it." +
                "||C1 Advanced is the in-depth, high-level qualification showing that a person has language skills " +
                "that employers and universities are looking for." +
                "||More information about the certificate can be found {0}",
        list: [],
        links: [
          {
            href: "https://www.cambridgeenglish.org/exams-and-tests/advanced/",
            desc: "here",
          },
        ],
      },
    ],
  });

  items.push({
    label: "2019",
    content: [
      {
        header: "Deutschlandstipendium (Stipend) 🏆",
        body:
                "On 27. November 2019 I was honored the Deutschlandstipendium sponsored by {1}." +
                "||The Deutschlandstipendium provides financial and non-material support to high-achieving and " +
                "committed students from all over the world. More information can be found on the {0}.",
        list: [],
        links: [
          {
            href: "https://www.deutschlandstipendium.de/de/english-1700.html",
            desc: "official website",
          },
          {
            href: "https://www.basf.com/global/en/topics/first-quarter-results-2021.html",
            desc: "BASF",
          },
        ],
      },
      {
        header: "AWS Certified Solutions Architect - Associate 📜",
        body:
                "On 05. August 2019 I passed the AWS Solutions Architect certificate." +
                "|More information about the certificate can be found {0}" +
                "||Abilities Validated by the Certification:",
        list: [
          "Effectively demonstrate knowledge of how to architect and deploy secure and robust applications on AWS technologies",
          "Define a solution using architectural design principles based on customer requirements",
          "Provide implementation guidance based on best practices to the organization throughout the life cycle of the project",
        ],
        links: [
          {
            href: "https://aws.amazon.com/certification/certified-solutions-architect-associate/",
            desc: "here",
          },
        ],
      },
      {
        header: "Bachelor's degree in Computer Science 🎓",
        body:
                "In July 2019, I graduated from the University of Applied Sciences in Mannheim " +
                "(bachelor, GPA: 3.6)." +
                "||Thesis: <i> Development of a concept to integrate MDF-4 in TensorFlow </i>" +
                "||Sadly, I cannot publish the thesis due to a non-disclosure agreement with {0} " +
                "(the company for which I wrote the thesis)." +
                "||Courses:",
        links: [
          {
            href: "https://www.vector.com/",
            desc: "Vector",
          },
        ],
      },
      {
        header: "Design Thinking Project - Fampedia 🧑🏻‍💻🌍",
        body:
                "During an international design thinking course, our team was tasked to develop a product that is " +
                "related to graveyards. We had some initial problems because our ideas for graveyards, " +
                "like for example a digital tombstone, all had the same problem: " +
                "When and how do we collect information about the deceased person? This lead us on the path of families. " +
                "After a lot of research and interviews, we came up with Fampedia. With Fampedia, " +
                "a family can create their own private space, where they can collect moments. " +
                "This information belongs to every family member and everything is saved for the future. " +
                "This makes Fampedia different from traditional social networks and helps to bring all generations " +
                "together. For example, less tech-savvy members can get help from other family members. " +
                "| | Sadly the {1} was shut after the project ended, but you can {0}. " +
                "|Or visit the {3} for more insights. || Technologies used:",
        list: [
          "Angular",
          "Express",
          "Docker",
          "MongoDB",
          "GitLab CI",
          "Sharp.js",
          "Socket.io",
          "AWS & Netlify Hosting",
        ],
        links: [
          {
            href: "https://github.com/PhilipOe1612340/Fampedia",
            desc: "find the code here",
          },
          {
            href: "https://fampedia.de",
            desc: "site",
          },
          { href: "https://angular.io/", desc: "Angular" },
          {
            href: "https://inno-space.de/projects/fampedia/",
            desc: "project page",
          },
        ],
        image: "fampedia.png",
      },
    ],
  });

  items.push({
    label: "2018",
    content: [
      {
        header: "Mittelstandsstipendium (Stipend) 🏆",
        body:
                "In October 2018, I was honored the Mittelstandsstipendium sponsored by {1}." +
                "||The Mittelstandsstipendium is a initiative of medium-sized companies " +
                "in cooperation with the University of Applied Sciences Mannheim. " +
                "More information can be found on the {0}",
        list: [],
        links: [
          {
            href: "https://www.hs-mannheim.de/die-hochschule/studium-und-lehre/studienfoerderung-stipendien/mittelstandsstipendien.html",
            desc: "official website",
          },
          {
            href: "https://www.vector.com/",
            desc: "Vector",
          },
        ],
      },
      {
        header: "Internship @ Fraunhofer CMA (Maryland, 🇺🇸)",
        body:
                "My fifth bachelor semester consisted of a 6-month internship at a company. " +
                "For this, I applied at the {1}, went through their interview process and got accepted :-)" +

                "||In retrospect, I am very happy that I got the chance to live and work in the US for 6-month. " +
                "It was a great time during which I learned so many things " +
                "(cs related, language related, working in an international team, etc.)" +

                "|| While I worked on multiple projects during my internship, there was one project that I was " +
                "assigned to from the beginning. Luckily it was also the most interesting (and challenging) one." +
                "|The name of the project, launched by IARPA, is {0} which is the short form for " +
                "<i>Functional Genomic and Computational Assessment of Threats</i>. Below a short summary:" +

                "||<q>The Functional Genomic and Computational Assessment of Threats (Fun GCAT) program intends to " +
                "develop new approaches and tools for the screening of nucleic acid sequences, " +
                "and for the functional annotation and characterization of genes of concern, with the goal " +
                "of preventing the accidental or intentional creation of a biological threat</q> - IARPA" +
                "" +
                "||While I was not actively developing the software, I was working one quality assurance. " +
                "So I helped the developers (of which many had a stronger biological background than a CS background) " +
                "with writing clean and consistent code and automating some of the repeating tasks (e.g. CI/CD). " +
                "I also developed a small test suite which exposed multiple bugs (even a few critical).",
        links: [
          {
            href: "https://www.iarpa.gov/index.php/research-programs/fun-gcat",
            desc: "Fun GCAT",
          },
          {
            href: "https://www.iarpa.gov/index.php/research-programs/fun-gcat",
            desc: "Fraunhofer USA Center Mid-Atlantic (CMA)",
          },
        ],
        list: [],
      },
    ],
  });

  items.push({
    label: "2017",
    content: [
      {
        header: "Project Semester - Botforge 🧑🏻‍💻",
        body:
                "At the University of Applied Sciences in Mannheim, the fourth semester is always something special. " +
                "For the first time students get to work with a real company on a real project " +
                "but in a save environment. Our task was it to build a platform for {0}, " +
                "a company that develops conversational commerce and AI software. Using this platform you were " +
                "supposed to be able to configure text bots that can then be deployed to interact with customers. " +
                "We worked for 10 weeks in a team of 4 design students and 6 computer science students. " +
                "Since we had never done anything on that scale before, everything was a little messy at first, " +
                "but we were still proud of what we had achieved in such a short time. |The finished code is a " +
                "little ruf around the edges but you can find it {1}. " +
                "||The technologies we used to make this happen were:",
        list: ["Vue.js", "Docker + Compose", "Node.js"],
        links: [
          { href: "https://www.liveperson.com/", desc: "Liveperson" },
          {
            href: "https://github.com/ChristianCoenen/Botforge",
            desc: "here",
          },
        ],
        image: "SEP.png",
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
