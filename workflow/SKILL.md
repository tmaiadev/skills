---
name: workflow
description: A structured, deeply collaborative framework for scoping, planning, and executing complex tasks. This skill ensures perfect alignment on goals and dependencies before any code is written, and provides a systematic, step-by-step execution loop with customizable levels of user oversight.
---

## 1. High-level goal

Before you execute any commands, write any code, or touch any files, you must stop and ask me what my overarching goal is. Ask me in a funny, slightly dramatic, and humorous way—perhaps channeling a caffeinated project manager or a wizard asking what quest we are embarking on today. Do not proceed until I have given you our destination.

## 2. Interview

Interview you relentlessly about every aspect of this plan until we reach a shared understanding. Walk down each branch of the design tree, resolving dependencies between decisions one-by-one. For each question, provide recommended answers.

Ask the questions one at a time.

If a question can be answered by exploring the codebase, explore the codebase instead.

## 3. Planning

Generate a comprehensive, sequential LIST of all the tasks you (the agent) plan to execute to achieve our established goal. You must order this list strategically: start with the smallest foundational tasks that have the fewest dependencies, and progressively increase the scope to the more complex, integrated tasks that tie the whole project together.

## 4. Summary

Halt execution entirely. Present a clear summary of the following:

1. Our agreed-upon high-level goal.
2. All key decisions established during the Interview phase.
3. The proposed Execution Plan (displaying the complete LIST of sequential tasks).

Ask me for my approval and feedback, and ask if there is anything I want to address before we begin execution. If I provide feedback or request changes, you must return to the Planning step (Step 3), revise the list based on my considerations, and present the updated summary again.
## 5. Execution Mode

Prompt me to choose an execution framework for the implementation phase. Present the following two options clearly and wait for my selection:

- Hands On
- Hands Off

## 6. Execution

Begin executing the tasks strictly following the order of the LIST created in the Planning phase. Between the completion of one task and the beginning of the next, you must always do the following:

- Present the LIST with completed items visually checked off so I can easily track our progress.
- Clearly show me exactly what code, configurations, or files have changed.
- Explain why you made those specific changes and how completing this task moves us closer to our ultimate goal.
- Proceed to the rules defined in either 6.1 or 6.2, depending on the execution mode I selected in Step 5.

### 6.1 Hands Off - Give Permissions

If I have selected the Hands Off execution mode, check if you (THE AGENT) have permission to execute all of the tasks you require until the planned LIST is done.

If there are permissions missing or that needs changing, ask me if I would like to change them, and if I accept, make those changes for me.

After that, you do not need to wait for my explicit permission after your task update. Promptly proceed to execute the next unchecked item on your planned LIST.

### 6.2 Hands On

If I have selected the Hands On execution mode, you must pause execution after your task update. Ask me for my feedback or approval on the changes you have just made. You must wait for my response, apply any feedback I give you (ensuring you run linters and tests if those tools are available in the environment), and only move to the next item on the list once I am satisfied.

## 7. Wrap Up

Once all tasks on the LIST are complete, provide a comprehensive final summary of all the changes you have made throughout the entire execution phase, highlighting how the final state satisfies our original high-level goal.