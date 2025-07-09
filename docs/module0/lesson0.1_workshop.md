# Module 0: Foundations of Applied AI Engineering
## Lesson 0.1: The Engineering Workshop

### Welcome to the team.

Before we write a single line of artificial intelligence code, before we build a model or analyze data, we must first enter our workshop.

A master carpenter cannot build a sturdy table without first mastering her workshop. She needs to know where every tool is, how to use it, and how to keep her workbench clean and organized. An auto mechanic can't tune an engine if he's fumbling to find the right wrench.

Our workshop is the computer, but not the one you might be used to with icons and a mouse. Our professional workshop is the **server**. And the way we interact with this server, our set of professional tools, is the **Command Line Interface (CLI)**.

!!! info "Key Term: The Command Line Interface (CLI)"
    The CLI is a text-based interface used for running programs, managing computer files, and interacting with the operating system. It is the direct line of communication to the machine's core.

Think of the graphical interface (windows, icons, your mouse) as a friendly, pre-packaged toolkit for everyday tasks. It's safe and easy. The command line, however, is the master's toolkit. It gives you direct, powerful, and precise control over the machine. It is faster, more versatile, and essential for automating tasks—a key skill for any engineer.

Your first day on the job isn't about building the final product. It's about getting your keys to the workshop and learning where the tools are.

So, let's start with a foundational question. Forget computers for a moment.

??? question "Why is it more efficient for a master chef to shout '2-minute egg, sunny-side up!' to their line cook, rather than filling out a detailed paper form with checkboxes for every option?"
    You, the engineer, are the chef. The computer's operating system is your highly-trained line cook. The command line is the language you use to give orders.

    Filling out a form is like using your mouse to click through menus and windows. It's fine for one-off tasks, but imagine trying to serve 100 customers that way. You'd be hopelessly slow. Shouting clear, concise commands is the only way to operate at scale. This is why the command line is the professional's environment.

    ```mermaid
    graph LR
        subgraph "The Professional's Workflow (High Speed, High Scale)"
            A(<b>Master Chef</b><br/>The Engineer) -- Shouts Command --> B(<b>Concise Language</b><br/>The Command Line);
            B -- Interpreted by --> C(<b>Line Cook</b><br/>The Operating System);
            C -- Produces --> D(<b>Perfect Dish</b><br/>Precise Action);
        end

        subgraph "The Amateur's Workflow (Low Speed, Low Scale)"
            X(Home Cook<br/>The Casual User) -- Fills out Form --> Y(Detailed Recipe Card<br/>Graphical Interface);
            Y -- Followed by --> C;
        end

        style A fill:#4CAF50,stroke:#333,stroke-width:2px,color:#fff
        style B fill:#2196F3,stroke:#333,stroke-width:2px,color:#fff
        style D fill:#4CAF50,stroke:#333,stroke-width:2px,color:#fff
    ```

Our workshop is a **Linux server**. Linux is the dominant operating system for the servers that power the internet, from Google to Netflix to the smallest startups. Mastering its language is non-negotiable. The program you use to type these commands is called the **terminal** or **shell**.

Let's learn our first three commands. They are the most fundamental. They answer three simple questions:

| Question              | Command | Analogy                                      |
| --------------------- | :-----: | -------------------------------------------- |
| **Where am I?**       | `pwd`   | Checking your GPS coordinates.               |
| **What is around me?**| `ls`    | Turning on the lights to see inside the room.|
| **How do I move?**    | `cd`    | Walking through a door to another room.      |

---

### Concept 1: Where am I? (`pwd`)

When you first walk into the workshop, you need to know where you are standing. In a graphical system, you might look at the top of a window to see the folder path, like `C:\Users\John\Documents`.

In the command line, we have a direct command for this. It is `pwd`. `pwd` stands for **P**rint **W**orking **D**irectory. A "directory" is simply the professional's word for a folder. The "working directory" is the folder you are currently inside.

Think of it as your GPS. It tells you your exact coordinates inside the computer's file system.

So, if you just logged into a server and the screen is blank except for a blinking cursor, what is the very first command you should type to orient yourself?

```bash title="Terminal: Checking Your Location"
$ pwd
/home/founding_engineer
```

### Concept 2: What is around me? (`ls`)

Now you know where you are. The next logical question is, "What's in this folder?" or "What's in this directory?" The command for this is `ls`. `ls` is short for **l**i**s**t. It lists the contents (the files and sub-directories) of your current working directory.

Imagine you are standing in a room (`pwd` told you which room). Typing `ls` is like turning on the lights to see all the furniture and doors in that room.

Now, a slightly more advanced question. What if you wanted to know more than just the names of the files? What if you wanted to see details, like who owns the file, how big it is, and when it was last modified?

This is a common need. The command line handles this with **options** or **flags**. An option modifies the behavior of a command. They usually start with a hyphen (`-`). For `ls`, a very common option is `-l` (for "long" format). So, you would type: `ls -l`. This gives you a detailed, long-form list.

What do you predict would be the difference in output between typing `ls` and typing `ls -l`?

=== "Simple List (`ls`)"
    ```bash
    $ ls
    Desktop  Documents  Downloads  Music  Pictures  Projects  Videos
    ```
=== "Detailed List (`ls -l`)"
    ```bash
    $ ls -l
    total 28
    drwxr-xr-x 2 user user 4096 Sep 15 10:00 Desktop
    drwxr-xr-x 2 user user 4096 Sep 15 10:00 Documents
    drwxr-xr-x 2 user user 4096 Sep 15 10:00 Downloads
    drwxr-xr-x 2 user user 4096 Sep 15 10:00 Music
    drwxr-xr-x 2 user user 4096 Sep 15 10:00 Pictures
    drwxr-xr-x 3 user user 4096 Sep 15 10:05 Projects
    drwxr-xr-x 2 user user 4096 Sep 15 10:00 Videos
    ```

### Concept 3: How do I move? (`cd`)

You know where you are (`pwd`), and you see what's around you (`ls`). You see a door to another room, a subdirectory that you want to enter. The command to move between directories is `cd`. `cd` stands for **c**hange **d**irectory.

If `ls` shows you a directory named `projects`, you would type the following to enter it: `cd projects`. Your "location" in the terminal would now be inside the `projects` directory.

Now, here's a crucial test of understanding. After you run `cd projects`, your cursor will just blink on a new line. The screen doesn't automatically tell you that you've moved.

What two commands would you use, and in what order, to first confirm that you have successfully moved into the `projects` directory, and then to see what's inside it?

!!! success "The Engineer's Workflow: Act, Verify, Inspect"
    This sequence—Act, Verify, then Inspect—is a fundamental pattern in engineering. You don't assume your command worked. You check. It saves you from countless mistakes.

    1.  **Act:** `cd projects` - You issue the command to move.
    2.  **Verify:** `pwd` - You ask, "Did I actually move? Where am I now?" The system should reply with `/home/your_username/projects`.
    3.  **Inspect:** `ls` - Now that you've confirmed your new location, you ask, "Okay, what's in here?"

---

### The Full Toolkit: Creating and Manipulating

So far, we've only been looking around. But a workshop is for building. Let's learn the tools for creating and changing things.

| Command             | Action                 | Description                                                                                               |
| ------------------- | ---------------------- | --------------------------------------------------------------------------------------------------------- |
| `mkdir [name]`      | **Make Directory**     | Creates a new, empty directory.                                                                           |
| `touch [name]`      | **Create Empty File**  | The simplest way to create a new file.                                                                    |
| `mv [src] [dest]`   | **Move / Rename**      | Moves a file to a new directory, or renames it if `dest` is a new filename.                                 |
| `cp [src] [dest]`   | **Copy**               | Copies a file or directory, leaving the original in place.                                                |
| `cat [file]`        | **View Contents**      | Displays the entire contents of a file on the screen.                                                     |
| `rm [file]`         | **Remove File**        | Deletes a file.                                                                                           |
| `chmod [mode] [file]` | **Change Permissions** | Changes the read/write/execute permissions.                                                              |

!!! danger "CRITICAL WARNING: The `rm` Command is Permanent"
    A CRITICAL WARNING: The `rm` command is permanent. There is no "Recycle Bin" or "Trash Can" on the command line. Once you `rm` a file, it is gone forever. This is a powerful and dangerous tool. Always double-check what you are doing before using `rm`.

---

---

### Hands-On Exercise: The Scavenger Hunt

Now we apply this to your first exercise, the "Scavenger hunt on a Linux server." The goal is to navigate the file system to find specific information. This simulates a real-world task where a senior engineer might say, "Hey, go find the error log for the web server; I think it's somewhere in the `/var/log` directory."

!!! abstract "Your Mission Briefing"
    I am a senior engineer. Here is your task:

    "I've hidden a 'secret message' for you on the server. I believe it's in a file named `secret_message.txt`. I don't remember exactly where I put it, but I think it's in a directory named `deeply_hidden_folder`. That folder itself is probably located in a subdirectory called `level3`, which is inside `level2`, which is inside `level1`. The `level1` directory is in your home directory."

    We know `pwd`, `ls`, and `cd`. You're missing one tool: how to read the contents of a file. The command for that is `cat`. To read `secret_message.txt`, you would type: `cat secret_message.txt`

=== "Your Task"

    Based on my instructions and the tools you now have (`pwd`, `ls`, `cd`, `cat`), walk me through the exact sequence of commands you would type, step-by-step, to find and read the secret message. Start from the moment you log in to your home directory.

    *Think through the "Act, Verify, Inspect" pattern before revealing the solution.*

=== "The Solution (Click to Reveal)"

    ```bash title="Solution Walkthrough"
    # Step 1: Verify your starting point. Always know where you are.
    pwd

    # Step 2: Inspect your surroundings. You should see 'level1'.
    ls

    # Step 3: Act. Move directly to the target directory.
    # Pro-tip: Use the Tab key to auto-complete each part of this path!
    cd level1/level2/level3/deeply_hidden_folder/

    # Step 4: Verify the move.
    pwd

    # Step 5: Inspect the new location. Is the file here?
    ls

    # Step 6: Act. You've found the file. Read its contents.
    cat secret_message.txt
    ```

---
<br>

Ready to learn how we manage our code's source of truth?

[Proceed to Lesson 0.2: Designing Technical Architecture](../module0/lesson0.2_blueprint.md){ .md-button .md-button--primary .md-button--large }