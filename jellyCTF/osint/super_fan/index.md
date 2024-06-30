# [osint] super_fan

Points: 955

Difficulty: hard

this guy is like some kind of jelly superfan or something... what a weirdo. he deleted all his old tweets and changed his username, can you find his new handle?

@j3llyfan7

note: unrelated to the stalknights challenges

10 point hint: pointer on where to start looking

20 point hint: info on how to use a piece of information further

30 point hint: specific location of the information required to complete

Author: arepi

<details>
<summary>View Hint</summary>

the profile page and some tweets can be found in the wayback machine, and those pages contain some metadata which will help you track down the new handle

also note that twitter's garbage JS will reload the page to tell you to login when viewing a profile on the wayback machine, but you can grab the HTML before that happens

there are some captures that are just broken too because of twitter, the latest for each should be working

</details>

<details>
<summary>View Hint</summary>

https://developer.x.com/en/docs/twitter-for-websites/web-intents/overview

</details>

<details>
<summary>View Hint</summary>

there are many IDs on the twitter page, but the one you want is found in either the profile banner URL on the profile page, or the `data-testid` property under the "Relevant people" sidebar's follow button on a tweet

</details>

<style>
details summary { 
    cursor: pointer;
}
</style>

##
