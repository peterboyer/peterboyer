### Hi! 👋

I'm a full stack web developer, currently working heavily with TypeScript.

---

#### esresult

🌟 Check out my latest project, [`esresult`](https://github.com/peterboyer/esresult).

- It's an awesome way to handle errors in your TypeScript projects in a type-safe and auto-completable way!
- Feedback welcome; especially about the structure/readability of the README!

> <details>
> 
> <summary><strong>Example</strong> (TypeScript) [Click to expand]</summary>
> 
> <br />
> 
> Annotate your function (with an success Value, and possible Error types):
>   
> ```ts
> import Result from "esresult";
>   
> function fn(input: string): Result<string, "InputEmpty" | "InputTooShort"> {
>     if (!input)
>         return Result.error("InputEmpty");
>     if (input.length < 10)
>         return Result.error("InputTooShort");
>     return Result(input);
> }
> ```
> 
> <br />
>                           
> Safely call your function (and work with a Result object):
> 
> ```ts
> const $ = fn("value");
>   
> const valueOrDefault = $.or("default"); // string
> const valueOrUndefined = $.orUndefined(); // string | undefined
> 
> $.error?.type // "InputEmpty" | "InputTooShort" | undefined
> 
> if ($.error) { return; }
> const [value] = $; // string (type-narrowed after `return` on error)
> ```
> 
> <br />
>
> Check out [the README](https://github.com/peterboyer/esresult) to learn more!
>   
> </details>

#### twitch

🎥 Come hang out when I stream [on Twitch](https://www.twitch.tv/peterboyer_/about)!

#### api design tips

📰 I like design; so much so I wrote [RESTful API Design Tips](https://github.com/peterboyer/restful-api-design-tips) (250+ stars!) Feedback welcome here too!

---
  
I hope you enjoy your stay, and please feel free to ask any questions. 😊
