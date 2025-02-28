# GUI Frame Diff  (AMOS WS 2023)

## About

**Library 1**

- It operates on the head unit (Android Auto), necessitating high efficiency.
- It processes a batch of images obtained from a single test run.
- Screenshots, encompassing all different system states, are generated on the head unit.
- A single video file is created from the batch of images received.

**Library 2**

- This library accepts two videos from two test runs as input.
- It calculates the difference between these two videos.
- The resulting image difference is then saved as a video.

**Library 3**
- Is the final GUI, that should look like a video editing tool  
- Can show the two input videos and the frame diff 

## Coding Guidelines 💅

- Use the Kotlin coding style defined here: https://kotlinlang.org/docs/coding-conventions.html
- Use ktlint to ensure a uniform coding style.

### Setup 

Install ktlint: https://pinterest.github.io/ktlint/1.0.1/install/cli/

We have a pre-commit hook that runs ktlint. Please activate it as follows:
1. Run `git config --local core.hooksPath .githooks` in the root directory of the project.
2. Mark the hook as executable: `chmod +x .githooks/pre-commit`

It makes sense to run `ktlint` more often to prevent a lot of formatting errors from piling up.
It is also encouraged to use an on-save formatter as provided by IDEs like IntelliJ, Android Studio and VS Code.
