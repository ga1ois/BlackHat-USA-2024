# BlackHat-USA-2024

Title:
Let the Cache Cache and Let the WebAssembly Assemble: Knockin' on Chrome's Shell

Abstract:

It is becoming increasingly challenging to exploit the Chrome browser with V8 JavaScript engine vulnerabilities. This is mainly due to the efforts of the V8 team constantly improving V8 security. In particular, there is a new in-process sandbox for V8 called V8 Sandbox, which is designed to prevent memory corruption vulnerabilities in the V8 engine from successful code executions even when exploitation primitives are available inside the V8 Sandbox. Recently, the V8 Sandbox beta version was officially released in Chrome M123, which introduced significant improvements that fundamentally broke all publicly disclosed escape techniques and their potential variants, making the V8 exploitation significantly more difficult.

This presentation discloses the full V8 exploit chain we used against Google Chrome and Microsoft Edge at Pwn2Own Vancouver 2024. This is a unique exploit chain that has successfully broken both V8 and V8 Sandbox, contributing to breaking the 3 year-period during which Chrome was not PWNED at Pwn2Own. We will start by unveiling how a single JavaScript object creation can trick the V8 JavaScript engine. From that, we will discuss the universal exploitation techniques we used to convert a single out-of-bounds (OOB) read vulnerability without any infoleak into a highly reliable exploit with close to a 100% success rate. Finally, we will share the details of our novel V8 Sandbox escape technique which worked across all existing Chrome versions and branches at the time, and differed from all previous techniques that relied on raw pointers inside the V8 Sandbox.

Link:
https://www.blackhat.com/us-24/briefings/schedule/index.html#let-the-cache-cache-and-let-the-webassembly-assemble-knockin-on-chromes-shell-39312
