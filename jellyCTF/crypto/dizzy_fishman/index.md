# [crypto] dizzy_fishman

Points: 896

Difficulty: hard

Sakana is sending some suspicious looking messages to Dizzy - looks like they're exchanging a shared secret key to encrypt the messages.

Alice has hacked into their key exchange system but needs more help with the exploit. Can you find a way to reveal their secret key and decrypt the message?

10 point hint: Algorithm/Area to focus on
20 point hint: Example that could work if it wasn't validated by the challenge

Author: Sheepiroo

`nc chals.jellyc.tf 4000`

<details>
<summary>View Hint</summary>

Diffie-Helman key exchange.

Challenge focus is on manipulating `g` to limit the possible values for the public and shared secret key.

Once the key is obtained, AES decryption can be done easily.

</details>

<details>
<summary>View Hint</summary>

g = 1 could work (if only the challenge didn't reject it)

If g = 1:

- (g^a mod p) = (1 mod p) = 1 for any value of a
- The public keys will always be 1 mod p
- The shared key will always be (g^a)^b mod p = 1^b mod p = 1

Is there a different `g` which also has a small number of possible public and secret keys?

</details>

<style>
details summary { 
    cursor: pointer;
}
</style>

Files: [dizzy_fishman.zip](./dizzy_fishman.zip)

##
