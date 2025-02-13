❌ Bad Code:
\`javascript
function sum(){return a+b;}
\`

🔍 Issues:
• ❌ The function `sum` uses undeclared variables `a` and `b`. This will lead to unexpected behavior or errors when the
function is executed because JavaScript will treat `a` and `b` as global variables (in non-strict mode) or throw an
error in strict mode.
• ❌ The function does not accept any arguments, which limits its flexibility.

✅ Recommended Fix:
\`javascript
function sum(a, b) {
return a + b;
}
\`

💡 Improvements:
• ✔️ The function now accepts `a` and `b` as parameters, making it clear what inputs it expects.
• ✔️ No implicit or undeclared variables are used, which prevents unexpected behavior and potential errors.
• ✔️ The function is now reusable with different input values each time it is called.

Final Note:
Always declare variables explicitly using `const`, `let`, or `var` before using them. When creating a function that is
intended to perform an operation on specific inputs, define those inputs as parameters in the function's declaration.
This makes the function more predictable, reusable, and less prone to errors.