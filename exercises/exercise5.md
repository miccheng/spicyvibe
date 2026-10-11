# Exercise 5: Vibe Code via Spec Driven Development

For more sophisticated applications (where you work with a team), you might want a more structured way.

## What is Spec Driven Development?

- Write and refine the specification of a system before (and alongside) implementing the code.
- The specification becomes the primary source of truth for what the software should do.

## Development Workflow

1. Define the behavior, requirements, interfaces, and constraints.
2. Review and validate the specification with stakeholders.
3. Implement code that satisfies the specification.
4. Test against the specification.
5. Update the specification as requirements evolve.

There are several frameworks for Spec Driven Development. Today, we will be using OpenSpec.

## Intro to OpenSpec

[OpenSpec](https://github.com/Fission-AI/OpenSpec) helps you and your AI coding assistant agree on what to build before any code is written. You describe the change, the AI drafts a short spec and a task list, you both look at the same plan, and then the work happens. No more discovering halfway through that the AI built the wrong thing.

We will be using some slash commands (`/<command>`) to operate OpenSpec.

The workflow we will use today:

```
/opsx-propose ──► /opsx-apply ──► /opsx-sync ──► /opsx-archive
```

## Build a weather app

1. Let's create a new project folder inide `videprojects` & `cd` into the new project folder.

    In Terminal / Console, type:

    ```bash
    mkdir weather_app
    cd weather_app
    ```

2. Initialize a fresh Git reposiotry in this folder to track changes:

    ```bash
    git init
    ```

3. Let's install [OpenSpec](https://github.com/Fission-AI/OpenSpec/).

    ```bash
    npm install -g @fission-ai/openspec@latest
    ```

4. Initialize OpenSpec in this project folder:

    ```bash
    openspec init
    ```

5. Select **OpenCode** as the tool.

    - Press `<up>` or `<down>` key to find `OpenCode`. 
    - Press `<space>` key to select the tool. 
    - Press `<enter>` to confirm the selection.

6. To open this folder in VSCode, type:

    ```bash
    code .
    ```

7. We'll be using some live weather data from [Data.gov.sg](https://data.gov.sg/).

    Go to each of the following site below and click on "Download API Specs" on each of the page. Save the files into the `weather_app` folder (i.e. `Desktop/vibeprojects/weather_app`).

    Name | Description
    ---- | -----------
    [24-hour Weather Forecast](https://data.gov.sg/datasets?formats=API&sort=relevancy&resultId=d_ce2eb1e307bda31993c533285834ef2b) | Singapore weather forecast API for the next 24 hours. Real-time data from the National Environment Agency (NEA) Meteorological Service Singapore (MSS). Ad-hoc updates may also occur outside the standard cadence.
    [Pollutant Standards Index (PSI)](https://data.gov.sg/datasets?formats=API&sort=relevancy&resultId=d_fe37906a0182569d891506e815e819b7#GET/psi) | PSI readings are provided for each major region in Singapore.
    [PM2.5](https://data.gov.sg/datasets?formats=API&sort=relevancy&resultId=d_e1058d6974c877257e32048ab128ad83#GET/pm25) | PM 2.5 readings are provided for each major region in Singapore.

    Feel free to read through these documents to find out what you can get from these APIs.

8. Start **OpenCode** from this project folder. 

    > _**Note:** Make sure to start a fresh OpenCode session._

9. In OpenCode, use this prompt:

    ```
    /opsx-propose "Build a Singapore weather app that will show me the weather, PMI and PM2.5 readings throughout the day. The OpenAPI Specifications for the relevant APIs are included in this folder."
    ```

10. OpenSpec generates a bunch of artifacts as part of its planning (i.e. a bunch Markdown files are created in the `openspec` folder. Review the Markdown files using VSCode.

11. Chances are, the proposal may be missing some things. Feel free to edit them in VSCode.

12. Once you are happy with the proposal, type (in OpenCode): `/opsx-apply` to start the implementation.

13. Sometimes things might stall. Just press `<esc>` twice and type: `continue` and press `<enter>` to continue where it hung.

14. You can also see its progress in VSCode. Can glance at `task.md` to see where its at.

15. Follow the on-screen instructions on how to run the Weather App

16. Once you are happy with this iteration, just sync and archive the work:

    ```
    /opsx-sync
    /opsx-archive
    ```

17. Let's commit the changes to Git. In OpenCode, type:

    ```
    Let's commit the changes to Git.
    ```

## Change request: Add Visualisation

18. Let's implement some visualisation.

    ```
    /opsx-propose "Let's beautify the app with some visualisation of the data. Let's use a vector map to represent singapore and the weather in different regions"
    ```

19. Inspec the proposed plan in the `openspec` folder. Review the Markdown files using VSCode.

20. Once you are happy with the proposal, type (in OpenCode): `/opsx-apply` to start the implementation.

21. View and verify the final implementation in the browser.

22. Once you are happy, can sync & archive the work:

    ```
    /opsx-sync
    /opsx-archive
    ```

23. Let's commit the changes to Git. In OpenCode, type:

    ```
    Let's commit the changes to Git.
    ```

## Troubleshooting:

If things get stuck, might be due to the application server running in the background.

```
pa aux | grep node
```

Find the process number and kill it:

```
kill -9 1234455
```

## Things to Ponder

- How do you feel about the level of detail exposed to you in the SDD approach?
- Do you have more confidence in AI implementing the right thing?
- How might you apply this to your team or workplace?
