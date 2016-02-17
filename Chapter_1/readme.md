##### Question:
If you type the exercise as it's written in the chapter, Rubocop will complain about the double quoted strings.  In the Readme.md for this directory, explain how you got rid of the offenses.  Did you fix the strings?  Or did you tell Rubocop to ignore those code style violations?  Why did you pick what you did?
#####Answer:
I chose to tell rubocop to ignore string literals to resolve the issue. I found my solution here: http://adadevacademy.tumblr.com/post/78135681910/how-to-get-rubocop-to-ignore-string-literals

Is that the correct solution?  I'm not sure.  The author states that this is a violation because Rails can sometimes cause conflicts with double quoted strings.  But he viewed that as a relatively small violation and worth the potential risk.  I don't know if that is the right solution or not...

To tell rubocop to ignore string literals, add the following to .rubocop.yml:

```
StringLiterals:
  Enabled: false
```


