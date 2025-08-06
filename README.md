# How-To-Upload-Files-On-Pipe-Network-Firestarter-Storage
This guideline shows how to partake in pipe network's referral program (to earn 100 PIPE per successful referral) &amp; also upload files on the network's firestarter storage.

## Open Command Environment
If you are unable to install Ubuntu on your Windows-based PC from the repository directly, check out this [guide](https://github.com/NotOlootu/How-to-Install-Docker-Manually-on-Ubuntu) for manual installation procedures.


## Install Pipe Client
```
bash <(curl -sSL https://raw.githubusercontent.com/pipenetwork/pipe/main/setup.sh)
```

<img width="1067" height="740" alt="image" src="https://github.com/user-attachments/assets/6a5d9b6b-85ec-4037-8a88-1f8dc9029b1b" />


## Create Profile
```
pipe new-user USERNAME
```

NOTES: Replace "USERNAME" with your choosen username

To edit the command script, you can copy, paste & edit in notepad
      
SAVE YOUR USER-ID, APP KEY & SOLANA PUBKEY
      
Although optional, I advise you set password

<img width="694" height="63" alt="image" src="https://github.com/user-attachments/assets/1dbc7e15-6e84-4c44-88d9-62ad12be999f" />


## GET FAUCET TOKENS

Copy the generated Solana Pubkey

Visit https://faucet.solana.com/

Claim minimum of 2 SOL (DEVNET). Connect github if necessary.


## Creating On-Chain Transaction (Swap)
```
pipe swap-sol-for-pipe AMOUNT
```

NOTE: Replace "AMOUNT" with the exact amount of SOL you want to swap, say 1 SOL, therefore "pipe swap-sol-for-pipe 1"

You need to swap a minimum of 1 SOL (DEVNET)

<img width="666" height="104" alt="image" src="https://github.com/user-attachments/assets/9571f802-d2de-4ce3-8bc3-ba2579abb3ec" />


## Bind Profile To Referral Code
```
pipe referral apply THINKPAD-XXHY
```


## Uploading Files/Folders
The aim is to upload a directory. You can choose to upload any directory of your choice. Although, the best choice would be to upload a directory that has personal file or data, you can just upload any of the folders in the installation directory.

### Option 1 (Uploading Files/Folders)

If uploading any folder in the installation directory, sensitive files (for examples, files that hold you user details) would be blocked from uploading automatically.

The first step is to check the directories in the installation folder. To do this, run
```
ls -l
```

<img width="656" height="142" alt="image" src="https://github.com/user-attachments/assets/083d81ca-8210-4002-a398-67c90dd78b14" />

The image above might differ from what you have which isn't a problem.

Depends on your choice, you can choose from one of the directories (excluding "wallet-gen" & "node_info.json") to upload 

Let's go a step further to narrow down the directory to upload. Let's open the "pipe" folder

```
cd pipe
ls -l
```

<img width="723" height="227" alt="image" src="https://github.com/user-attachments/assets/c94a7d41-4e3b-41c2-acf8-8c80e2020105" />


Okay, we can upload the "target" folder

```
pipe upload-directory target
```

<img width="1070" height="224" alt="image" src="https://github.com/user-attachments/assets/d50d8f28-9a10-4d21-aba6-e828720056d0" />


### Option 2 (Uploading Files/Folders)

Copy any folder of your choice from your local drive, then paste in one of pipe's installation directory. You can paste in the "target" folder we used in option 1.

NOTE: The "target" folder is now our parent folder, so we must locate & open it in the command environment before we can upload our chosen file/folder

```
cd pipe/target
ls -l
```

Then

```
pipe upload-directory FOLDER-NAME
```

# That's it.

Repeat the swap & upload process as much as you can.


### Appendix

If you run into any problem after creating your profile, then logout & login back

To logout

```
logout
```

To login

```
pipe login USERNAME
```

To generate your referral code

```
pipe referral generate
```


Reference (https://github.com/PipeNetwork/pipe)

Kindly follow me on [twitter](https://x.com/journeyer_dunya) for more hacks & updates.
