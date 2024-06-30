# [web] vlookup_hot_singles_2

Points: 911

Difficulty: hard

oh. it's her. well, see if you can get the flag at /app/flag.txt and then get out of there

10 point hint: tooling recommendation/where to start looking

20 point hint: useful info for figuring out the vulnerable codepaths

50 point hint: explicit place to attack and code to do so

Author: arepi

https://vlookup-hot-singles.jellyc.tf/ 


<details>
<summary>View Hint</summary>

some of the libraries are at a specific version for a reason. try using something like https://github.com/aquasecurity/trivy to see if there's anything interesting worth exploiting

</details>

<details>
<summary>View Hint</summary>

openpyxl uses lxml only in a few specific places

</details>

<details>
<summary>View Hint</summary>

CVE-2017-5992 XXE in `docProps/core.xml`. pocs exist on the internet

</details>

<style>
details summary { 
    cursor: pointer;
}
</style>

##
