---
tags:
  - Tools
date:
  created: 2024-09-04
---

# Cursor: Features that may be missed

## AI Models

It's important to note that Cursor utilizes different models for various features. Understanding this allows you to select the appropriate model and use the right functionality to accomplish your tasks effectively.

<div class="grid cards" markdown>

- :robot: **Tab model** <br> Cursor's own model for code completion
- :speech_balloon: **Chat model** <br> Third-party models (e.g., Claude 3.5) accessed via API
- :keyboard: **++cmd+k++ model** <br> Third-party models (e.g., Claude 3.5) accessed via API
- :zap: **Fast apply model** <br> Cursor's model for speeding up full file code generation using speculative decoding

</div>

!!! info "Learn More"

    For detailed information, refer to the [Cursor Models documentation](https://docs.cursor.com/advanced/models).

<details>
<summary>Fast Apply Model Details</summary>

The fast apply model uses speculative decode to accelerate the generation of code for entire files, resulting in faster diff production. <a href="https://www.cursor.com/blog/instant-apply">Read more about Instant Apply</a>.

</details>

## Partially TAB

1. Enable the feature

    - Go to Cursor Settings → Features → Cursor Tab
    - Set "Partial Accepts" to enabled

2. Use ++cmd+right++ to partially accept code

## AI Review (Beta)

AI Review allows you to get AI-powered feedback on your code changes. It can analyze your working state, diff with the main branch, or your last commit.

### Key Features

- :mag: Customizable review focus
- :computer: Multiple review options
- :speech_balloon: Interactive chat for more information

### How to Use

1. Enable AI Review in Cursor settings
2. Choose a review option

    - Review Working State
    - Review Diff with Main Branch
    - Review Last Commit

3. Optionally, provide custom review instructions

!!! example "Custom Review Instructions"

    Prompt: focus on the performance of my code

!!! info "Learn More"

    For detailed information, visit the [AI Review documentation](https://docs.cursor.com/advanced/ai-review).

## Shadow Workspace

Shadow Workspace is an innovative feature that allows AIs to iterate on code in the background without affecting the user's workspace.

<div class="grid cards" markdown>

- :ghost: **Hidden Iteration** <br> AIs work in a separate, hidden environment
- :computer: **Full Development Environment** <br> Access to lints, go-to-definitions, and code execution
- :lock: **User Experience Protection** <br> Your coding experience remains unaffected
- :warning: **High Memory Usage** <br> Requires significant RAM for shadow workspace

</div>

!!! note "Technical Implementation"

    Shadow Workspace uses hidden Electron windows and plans to implement kernel-level folder proxies for enhanced functionality.

<details>
<summary>Learn More About Shadow Workspace</summary>

Shadow Workspace aims to provide AIs with a full development environment while maintaining independence from the user's workspace. This allows for more effective code generation and iteration.

For an in-depth look at the technical details and future plans, check out the <a href="https://www.cursor.com/blog/shadow-workspace">Shadow Workspace blog post</a>.

</details>
