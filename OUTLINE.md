# Golang Meetup Lightning Talk

 I am going to broadly speak about my journey in LLMs, using their code generation, multi-modal, and world understanding in interesting experiments, but through the evolution of the thinking now use it for practical work.   I have 15 minutes to speak.  Create a presentation with presenter notes.  It has a timeline to it, put a horizontal gauge of the progression from Nov 2024 to Jan 2026 in the upper right (don't make it flashy, it just conveys information as we go along.

## Nov 2024 TUI and multimodal models 

 From November 2024 working on [OllamaTea components](https://github.com/NimbleMarkets/ollamatea/tree/main?tab=readme-ov-file#ollamatea---bubbletea-component-for-ollama) and then using with `dbn-go` DataBento library make a  [NTCharts with OllamaTea  Multi-Modal inferencing demo](https://github.com/NimbleMarkets/ollamatea/blob/main/cmd/ot-timechart/README.md#databento-data-example).

## Apr 2025: MCP Exploration 

In April 2025, I dove in MCP servers with DataBento, buttplug-mcp, culminating in [Agent `dank-mcp`](https://github.com/AgentDank/dank-mcp).  
From MCP creation, I learned that tool descriptions are most important, LLMs like structure which we can deliver in markdown, and that APIs are not necessarily meant to be wrapped.

## May 2025 MCP Agent Looping

I then had agentic loops developing that and  [screentime-mcp](https://github.com/AgentDank/screentime-mcp).  From AgentDank and ScreenTime MCP,  the lesson is taking world knowledge and lean on SQL to get deterministic answers to datasets and then agentic loop to improve it.  I was also in an agentic loop fixing up Charmbracelet Crush to use of MCPs while  using Crush to develop my MCP servers.  

## Nov 2025  AntiGravity + Gemini 3 and Opus 4.5 

in November 2025 , the power of AntiGravity with Gemini 3 Pro, alongside Claude Opus 4.5.   Where before making a webpage for AgentDank age verification took hours and nothing useable, Gemini one-shotted the verification page and an entire mocked chat interface, wherein i was then able to explore my idea right away.  I even one-shotted a DBA environment with embedded DuckDB wasm and 3D WebGL charts of cannabis data, from the time between the train.

## Mid Dec 2025: Vibe Coding for Kids

Before break, i was substitute teaching and the kids were just in google classroom so i vibe coded on the smartboard a [quadratic formula explorer](https://github.com/ConAcademy/quadratic_explorer) and  in honors geometry a [proving parallelgrams](https://github.com/ConAcademy/proving_parallelograms) web app.  I sprinkled some inspiration about machine intelligence.

## Late Dec 2025: MultiModal Debugging the Parallelogram

My friend later pasted an error with a bowtie shape and i used multimodal capabilities to automatically see the error from the image, create a fix, create a test for the fix, run the fix itself in chrome manipulating the page, screenshotting that and giving me a report.

## Late Dec 2025: Vibe Boat Engineering 

Since then, I was using the multimodal capabilities of Claude to help me engineer an improvement to my boat.  By describing the issue and giving it pictures of the CAD drawing, it could help solve structure configuration and implementation issues, such as screw diameters, materials selection, stress points.

## Jan 2026: Swift To 3D Model

  A few days later i saw the [Cadova](https://github.com/tomasf/Cadova) parametric modeling in Swift-to-CAD library for generating 3MF and  mid-comment on HackerNews, I realized i could use Swift as a ground truth for 3D models, the same was claude generates Docx for documents or SVG for images, and I vibe coded creating models!  

I started with Claude Desktop, but got into it with Claude Code.  I documented everything in my [WeaselToonCadova](https://github.com/ConAcademy/WeaselToonCadova) repo.

## Jan 2026: LLM-assisted renaissance
So many threads!
* NTCharts: adding multimodal and terminal testing infrastructure and using world understanding to [charting fix bug] (https://github.com/NimbleMarkets/ntcharts/issues/7)
* Moving OSS devops from Travis to GitHub Actions
* improving AgentDank go codebase and devops (`dank-extract`, snapshots)
* Create a Swift app that embodies the WeaselToonCadova loop
* HyperCube Vision app with mesh shaders
* booba: ghostty-web and BubbleTea components (see also `sip`)
* choosing a presentation and the presentation itself
* business and financial planning

## Jan 2026: Artistic License

I knew I was going to do this talk, and I appreciate Fallthrough on a lot of so I had the idea to flex my artistic side, which I consider much of my tech and life work to be art.

I started with a picture of the fallthrough hosts (i will paste it) and then asked it to iterate.   i then gave it another picture that included various other hosts and their names.  I asked it to find the original hosts in that picture and fine tune the models on that.  I also correctly identified the hosts.

The whole thing is nonsense, but we did it!    Here's the final model, and I 3D printed it!   I love the aesthetic of tree  support materials and I think it's a fitting conclusion to the various forms of computational graphs, models,  codepaths, coordinate spaces, algorithms, even path planning and gcode, to get this to manifest. 
---
Please take this stuff and solve your problems with it!