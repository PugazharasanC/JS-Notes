# Async/Await: Scripting the Next Blockbuster 🍿🚀

## Keywords Async and Await

In the realm of JavaScript, enter the dynamic duo: `async` and `await`. These keywords team up to revolutionize asynchronous programming, much like the lead pair in your favorite action-packed blockbuster. Let's uncover their roles in our coding saga.

# Async Function: The Prologue of a Cinematic Code Tale 🎬

In the vast script of JavaScript, an `async` function emerges as the protagonist—an asynchronous hero ready to unfold a captivating tale. Let's dive into the prologue of our cinematic code journey with an `async` function.

```javascript
// Async Function Definition
async function getMovieTitle() {
  return "Mankatha";
}

// Calling the Async Function
const movieTitlePromise = getMovieTitle();

console.log(movieTitlePromise);
```

## The Async Hero: `getMovieTitle`

Meet our Async Hero, `getMovieTitle`. This function is marked as `async`, signaling its prowess in handling asynchronous tasks. Its mission: retrieve the title of an epic movie—let's call it "Mankatha."

## Action Begins: Calling the Async Function

The script, eager to reveal the movie title, calls our Async Hero—`getMovieTitle`. But here's the twist: instead of immediately getting the title, it receives a Promise in return. The plot thickens!

```javascript
console.log(movieTitlePromise); // Promise {<fulfilled>: "Mankatha"}
```

**Output :**
```javascript
Promise {<fulfilled>: "Mankatha"}
  [[Prototype]]: Promise
  [[PromiseState]]: "fulfilled"
  [[PromiseResult]]: "Mankatha"
```

## The Promise: A Glimpse of the Future

`movieTitlePromise` holds a Promise—a commitment from our Async Hero that the movie title will be revealed. The script, undeterred by the asynchronous nature, patiently awaits the outcome.

## The Climax: Logging the Output

Asynchronously, when the movie title is ready, the `then` method steps in to capture the climax. It logs the awaited movie title, giving closure to this part of the code tale.

```javascript
movieTitlePromise.then((title) => {
  console.log("Movie Title:", title); // Movie Title: Mankatha
});
```

The log statement unveils the movie title, bringing the prologue to a satisfying end. In the upcoming acts, we'll delve into more complex plotlines, exploring the full potential of async functions. Get ready for an exciting code narrative reminiscent of your favorite cinematic adventures! 🚀🎥

```javascript
// Async Function Definition
async function playSuspensefulMusic(minutes) {
  console.log("Enchanting suspenseful music echoes...");
  return new Promise((resolve) => {
    setTimeout(() => {
      console.log("Suspense Revealed");
      resolve("Vinayak Mahadev and Prithvi walk away with bags of money");
    }, minutes * 60 * 1000);
  });
}

// Async Function Call
async function climaxScene() {
  console.log('Vinayak whispers "Action King" over the phone');
  const result = await playSuspensefulMusic(3);
  console.log("Climax Revealed:", result);
}

// Initiating the Climax Scene
climaxScene();
```

## The Setup: `playSuspensefulMusic`

Our script orchestrates the scene with an asynchronous function named `playSuspensefulMusic`. This function simulates enchanting suspenseful music and introduces a promise-based time delay to build anticipation.

## Action Unfolds: `climaxScene`

The protagonist, `climaxScene`, steps in to initiate the suspenseful sequence. It whispers the phrase "Action King" and eagerly awaits the outcome of `playSuspensefulMusic` using the `await` keyword, adding a touch of cinematic tension.

## The Suspense: Awaiting the Outcome

As the suspenseful music echoes, the `await` keyword gracefully pauses the script, allowing it to patiently await the resolution of the asynchronous `playSuspensefulMusic` function. The countdown begins!

## Climax Revealed: Logging the Result

Finally, the suspense is unveiled, and the script continues its execution. The result of the suspenseful theme music is captured in the variable `result` and is then vividly logged.

**Expected Output:**
```javascript
Vinayak whispers "Action King" over the phone
Enchanting suspenseful music echoes...
Suspense Revealed
Climax Revealed: Vinayak Mahadev and Prithvi walk away with bags of money
```

The script crafts a cinematic experience, complete with suspense, anticipation, and a climactic revelation. As we explore more scenes in the upcoming acts, be prepared for a riveting code tale that mirrors the excitement of your favorite cinematic adventures! 🍿🎬✨

## Navigating the Cinematic Code Tale: Try-Catch Chronicles 🍿🎬

In the ever-evolving script of JavaScript, the plot thickens with the introduction of error handling using `try` and `catch`. Let's embark on the next chapter of our cinematic code journey, exploring the intricacies of these constructs.

## The Unpredictable Plot: `unexpectedTwist`

In the ongoing cinematic code tale, our script introduces an `async` function named `unexpectedTwist`. This function represents a critical plot point, where the storyline could take an unexpected turn—either leading to the hero's success or presenting an unforeseen obstacle.

## Dive into the Unknown: `continuePlot`

The protagonist,

 `continuePlot`, steps in to navigate the uncertain plot. The `try` block encapsulates the asynchronous call to `unexpectedTwist`, aiming to capture the outcome. However, the `catch` block stands ready to handle any plot twists or unexpected challenges that may arise.

## The Drama Unfolds: `try` Block

Within the `try` block, the script awaits the resolution of `unexpectedTwist`. If all goes well, and the hero prevails against the odds, the outcome is captured and vividly logged. This represents the success path of the storyline.

## Plot Twist Unveiled: `catch` Block

In case of an unforeseen obstacle disrupting the plot, the `catch` block gracefully catches the error, preventing it from derailing the entire script. The error is logged, adding depth to the narrative, and the script proceeds with grace.

Now, let's explore the code that brings these elements to life.

```javascript
// Async Function Definition
async function unexpectedTwist() {
  return new Promise((resolve, reject) => {
    const randomEvent = Math.random();

    // Simulating an unexpected event (error or success)
    if (randomEvent < 0.5) {
      console.log("The plot takes an unexpected twist!");
      resolve("The hero prevails against all odds");
    } else {
      console.log("An unforeseen obstacle disrupts the storyline!");
      reject("The hero faces a sudden challenge");
    }
  });
}

// Async Function Call with Try-Catch
async function continuePlot() {
  try {
    const outcome = await unexpectedTwist();
    console.log("Outcome:", outcome);
  } catch (error) {
    console.error("Plot Twist Error:", error);
  }
}

// Initiating the Next Scene
continuePlot();
```

**Expected Output (Example):**
```javascript
The plot takes an unexpected twist!
Outcome: The hero prevails against all odds
```

or

```javascript
An unforeseen obstacle disrupts the storyline!
Plot Twist Error: The hero faces a sudden challenge
```

The script, equipped with try-catch error handling, ensures that the cinematic code tale continues seamlessly, adapting to unexpected twists and challenges. As we progress through the subsequent scenes, anticipate more plot developments and twists in this thrilling coding saga! 🍿🎬🌟