# Exercise 2: Start and Configure OpenCode

1. Make sure you are logged in to an OpenCode account (its free to create a [OpenCode Console](https://opencode.ai/console) account).

    - Type: `opencode auth login opencode`
    - Select: `OpenCode Console account`
    - Create or login to your OpenCode account.
    - Click on `Authorize` on the OpenCode website.
    - You should see:

        ```
        Device authorized
        You can return to your terminal.
        ```
2. In the Terminal / Console, make sure you are in the `vibeprojects` directory.

    > _**Tip:** Use the commands showns in [Exercise 1](./exercise1.md)._

3. To start OpenCode, type: `opencode`

4. Select one of the free AI models:

    - Type: `/models`
    - Select one of the Free models. 
        > _**Note:** The list of available free models may vary depending on OpenCode's service load. Just pick anyone that's available today._

5. Initialize the project folder: Type `/init` and press `Enter`.

    This creates an AGENTS.md file, which is the "brain" OpenCode uses to understand your specific codebase.

6. Try to prompt for something:

    ```
    How many "R"s are there in the word strawberry?
    ```

    You should see a response like this:

    ```
    There are 3 "R"s in the word "strawberry".
    The words break down like this:
    - s-t-r-a-w-b-e-**r}-{r}-y
    All three "r"s appear as part of the spelling of these berry-related words.
    ```

## Pro-Tip: Using a Paid AI Model

Once you get more experienced, you can also choose some other paid models.

1. Press: `ctrl` + `p` to access the **Commands** option.

2. Select `Connect Provider` to connect to a LLM (Large Language Model) provider.

    > **Pro-Tip:** Type `/connect` to get to this command

3. Select one of the Providers.

4. After you have connected to your LLM provider, go to **Commands** option and select `Switch Model` to select your LLM model.
