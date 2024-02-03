## Linux Assignment 4 

**1. Create a directory named "MyFiles" in your home directory. Navigate into this directory and list its contents.**
```
mkdir Myfile
```
![](https://lh7-us.googleusercontent.com/UH6LcbxoMrW2cgGZCvq9heRI7kqHiGFdhLN2Luwu3jTG8Wnd2MO-SxoHUMWhtLBZ4h0hgSHP2ImTHTnWBS2DSJj7XyrMhc5js8V03neQPa6HlE8SY6R_J4Ctc4GRBGJyW_4e5lFn4HCcyi-LJApXqRA)

**2. Copy a file named "document.txt" from your home directory to the "MyFiles" directory. Move the file to a subdirectory named "Documents" within "MyFiles."**
```
touch documents.txt
```
```
cp document.txt Myfile/
```
```
mkdir Document
```
```
mv document.txt Document/
```
```
ls Document/
```
![](https://lh7-us.googleusercontent.com/himn3I_jEzbgBuqdtCiHC15OWevnFT9xl-ZsB2dQpqpy0jUOsga5bF-WtrzsXIeP-rMJKNt7vGTvMMPgJtG1az7-gecr3JiAZ7-xhA9XHkLu3JMWl0ksembilfnXF5zFmNJG76tV5y_LWsoT_iupiS0)

**3. Create an empty file named "notes.txt" in the "MyFiles" directory. Afterward, delete the file.**
```
touch notes.txt
```
```
cat notes.txt
```
```
rm notes.txt
```
![](https://lh7-us.googleusercontent.com/fB_HLWagPdCDF4hftzOY0hEvBi_WzRXW1Cuc8_RSn99eU93BQQHrbDKZQiuU-gL1-wksGvMG_9P6Tf016HduteiT6upGohrPA7qrmC9urFvD_iWYkmoprjmsRDt5KuQeXVB8osjUzh1fEVUcTxKDYaI)

**4. Create a hard link named "hardlink.txt" for the file "document.txt" within the "Documents" subdirectory. Also, create a symbolic link named "symlink.txt" in the same location.**
```
ln document.txt Myfile/Document/hardlink.txt
```
```
ln -s document.txt Myfile/Document/symlink.txt
```
```
ls Myfile/Document/
```

![](https://lh7-us.googleusercontent.com/nsF2rPErZaKWTdvhJrcQoyWnLqsuDjz58UwNH9klGbxxpZ61Y1khArw9pqkQrcVlj12iFQ6yefm7p0dxPyOSxHA5rVqmzh5hQc5v7cJJmUyp4Aez1Lvq3wdxZT0kE_BHQ1tsjuyEGjXcTa_ZaKJeFcA)

**5. In the "MyFiles" directory, use a single command to list all files that start with the letter "a" and have a ".txt" extension.**
```
touch arav.txt arun.txt anmol.txt
```
```
 ls a*.txt
```

![](https://lh7-us.googleusercontent.com/sDSrDLICCMA1nEaW8hfVzkvbUYtBLCom5pvjB7ZgMCXuu5za2ePBfQiuWrDDGiZhD7TulVgvggt6ZinFwP-6540j3mTUh_ZtqO53Al5SjjsnG_q1kkwukpdIWdD3MAb3Z3GT0nXMb6T8PHdqArhDr1s)

**6. Rename all files in the "Documents" subdirectory of "MyFiles" with a ".bak" extension. Ensure the original file names are preserved.**
```
sudo vim rename.sh
```
```
cd Document/
```
```
 sudo bash ../rename.sh
```

![](https://lh7-us.googleusercontent.com/CC_3qe_Vk8lhR4EKwZYjlG9lghbXjug7Gb2lCbaUidEsXZdDw1Cn0C55rSIwKyrnW-E0_xkJ_-JY5qUzP0y3mlsZR0tjs6lKdszaIymzaIJg54saMLXHp4-2oiK30oZ3TRUHQQzQPVtdL8wkB--ti1I)

![](https://lh7-us.googleusercontent.com/KDAMESNLbIZ-pXT_TD9m2D7nPjzAfk9Y2yKMF766qi9nUdIaSy4t3SUwXuD2nUxu7azYlnfHtQeVjkRYgApHw2q_oxyj7Nxj8ZN8hrucPctQsPoxOVKkpGfb2IvZgTtwX_zWywocsjSBEHRVRawoDtg)

**7. Use a wildcard character to copy all files from the "Documents" subdirectory of "MyFiles" to another directory named "Backup."**
```
cp */home/vivek/Myfile/backup/
```
```
cd backup/
```
![](https://lh7-us.googleusercontent.com/Yd6Md0QjVlUMEZcxysR5srxjX3sZVkDrzmhVrTXhGLiwI2zaCpMowpPvy-RDNb6uvBlRliU5xQd2HV0E3SFFE4aA0y8sg65kXzMSvmeM_0JjbwLhVGhylM25VgUEHgMeJgn-7MoUvBpwtN-JLm3KkJ4)

**8. Execute the ls command to list files in the current directory. Save the output to a file named "file\_list.txt." Then, use a pipe to filter the output through grep to display only files with a ".txt" extension.**
```
 ls > file_list.txt**
```
```
cat file_list.txt | grep .txt
```

![](https://lh7-us.googleusercontent.com/dBdkTRN9SzQwazFWQxPUzvF12uq1UwVKzjgsm9iIiZpNDYBKViuwyXQ3YO9N_YB_O2TjDmCfhozSGCYpzPwfVgd_hv5gbOLsLcPJjakdJ_wZJ8Ap5mTkW3wQhm_ez7uOp6rEQegq8V_pfwGYhPAi8o4)

**9. Create a new text file named "my\_notes.txt" using the touch command. Open the file in the Vim editor, add some text, and save the changes.**
```
touch my_notes.txt
```
```
vim my_notes.txt
```

![](https://lh7-us.googleusercontent.com/pCR33jx8BckwnYlN2tr59_fHqrbQ3UPBgEUfkKE1MA7Huy7Ze0FaENm41PXpOK4nprccraLYfaxOqqGaKCiKtCXObrAcCGBMpKHMUyhhqyyKHy9grcwnxzqYFE6eEeYU-IN0ocH8uImSS20OXccB2ls)

**Add some tests and save the file.**

![](https://lh7-us.googleusercontent.com/z6zrtvy9YXhyp1w2k_opj--TZ3P3xHyze20zQhNafNvj377FDU8P4Cnbf91OmsQ7et-us4RAKE9Ur495rog_kqLA-5S-SSW0X_ogPAwPSG48b0ipUMdlUuTMSkjOjQRdz_QI2FNQtYnfT8l9lf3DrrQ)

![](https://lh7-us.googleusercontent.com/O5lGsu0By0Sx5TNdKXQeTHA7uNoS0x4B32bIAZGHdpaOfRJgzF6aBavms3IwEUU6Jn7guXHj1qwl0MFEjv3kur4MiX28QbnUx56yiEdgNcxcBw6aUtNgxnyg8etDVQvwIU4A3kiGpsNyJKR-wIajXSk)

**10. Run the date command and store the output in a variable named "current_date." Display the value of the variable and append it to the "my_notes.txt" file.**
```
current_date=$(date)
```
```
echo "current date : $current_date"
```
```
echo "$current_date" >> my_notes.txt
```

![](https://lh7-us.googleusercontent.com/1hQbj1pklfMKnz_kqc0gxgaOskfW2Iv9eESfZIW-Ep4Shd96XWoEas6GYm9t5fygSbiEy8GA15YufBfumYdAUtJ7ZpUjnMWZOygZy1rGJ0v14CbTuwpuER296wLdRSpJXfeajQU1K9lf_I30WtE_Wpk)


**11. Edit the Bash startup script (e.g., .bashrc) to set an environment variable named "CUSTOM_PATH" to a specific directory path. Ensure the variable is available in new shell sessions.**
```
vim .bashrc
```
```
source ~/.bashrc
```
```
echo $CUSTOM_PATH
```


![](https://lh7-us.googleusercontent.com/Ci9GJRPD0oW_pdWKyjxBOT-6N3kTSo3CzDonkTlt8aUYNobuWaqgGsg9UNEdjkKysb9xZYjvEPgwIHfQhINE704uu9lCgua6cHml1D6KnXvedEyjbfIo7OWXYAhVmDfkPMsL4sdAs6AaECrLYqmuBQs)

![](https://lh7-us.googleusercontent.com/n5HbiUogSjWqT-3tgsurfkgw0JLyENCx51xVpmp4msxfx6T1YnGHSVKTd-Qrhnuhc981f-r1MTkurzyr5VBO15ar0KzhK3oUcXuj9hmBGDdkwa_j-S8tXOiSOj7PXySOnO9WrdOSxas4HxdXPRNQWmM)


**12. Use the echo command to add a new line of text to the "my_notes.txt" file without overwriting existing content. Verify that the new text is appended.**
```
echo "how are you" >> my\_notes.txt
```
```
cat my_notes.txt
```
![](https://lh7-us.googleusercontent.com/pY9AJ1EX8YNUdrDMX0uXrv9XwaA2IDgHyGe2CwBXk3CvNdiNORVoDqhGNcWUjNIlHjPvDGMBxAIBAQIFCi_UnkGWUOBNmS2AVCXXXXVq0-sMPhSTxKeTFhgL1Is2AmydZjdZ-s3Hxw1jYRVjN_O5bxY)

**13. List all files in the "/etc" directory, filter the output to include only those containing the word "conf," and save the result to a file named "conf_files.txt."**
```
ls /etc | grep "conf" > conf_file.txt
```
```
cat conf_file.txt
```


![](https://lh7-us.googleusercontent.com/cYWWABlIMlc7JXo17m9ZTNHpJE284wLE2b_ZSbxwJGljKRUPABjWOiQSDWNj2Pg8rtvFGeuf3j-Y0t6GgtpUwgRjtb0hqlCSledN8-NvIVdzt-3LTXyXQEP41oiKnRreT8xEFZzZOxax3UQWSCkc3Qo)

**14. Open the "my_notes.txt" file in Vim. Use Vim's search and replace functionality to replace all occurrences of the word "important" with "critical." Save the changes.**

```
 vim my_notes.txt
```
```
:%s/important/critical/g
```

![](https://lh7-us.googleusercontent.com/_j0zI0Pmcy5SFUYoAeDnOhXU7-fcGcE6FpIJEIeNOW7n3cyL0G3PThmYzC12Xb75Bib30zwDZARK80SgKQMWh_5_O2JLdYKEMJGmYOH0PRClVcZt90RyipSVM3SO4FY8axGpSulTMj5SjRXu-ERPpK8)

![](https://lh7-us.googleusercontent.com/4i8aNMKt45CHiLvBQTJlJFbB_Der17B1fHIQ8kDDcePy8rnLpUmwl2ATRyCtt6z7blsxZmd0lFQuaRHi7DBmf-nhSXXMChKBiqfSo6rzDhD6Yov0cs6bXJXLK7jGTZ8CugPdUIHl-UuTfQeL0dQ-wM4)

**15. Create a new user account named "john_doe." Set the user's home directory to "/home/john_doe" and assign the user to the "users" group.**
```
sudo useradd -m  -d /home/john_doe -g users john_doe
```
```
ls /home/
```
```
ls -l
```

![](https://lh7-us.googleusercontent.com/P-RsyEkUAA7q6_2X6ibTgHe7JU3UwR83rUH_9Lmeu4mW2DGRfLdXRTeddEVoUAlXv7LzxbfVZWxcObZEXA0a0AlCxcs1UntbjX-R8ngGPiIzBTAx6GcmV5KEd39IlLqysj3RFtU5NPoWANqIuZnd8nk)

![](https://lh7-us.googleusercontent.com/h-s0hVJgGrE34Bllgyw_q9xEqWRGxw9DqjLk9MRWusR-6fEcl8ol9fwqifozYp5Kksuze7cSwzrtBFFyOzsFsOKpT9hBttftl4i_20qU4idAwGTKA7QL0wutUggxYblCjFjvL2V7NFWoWiY-72fNOgE)

**16. Add the user "john_doe" to the sudoers file, allowing them superuser privileges. Confirm that "john_doe" can execute commands with sudo.**
```
sudo usermod -aG users john_doe
```
```
id john_doe
```
```
su - john_doe
```
```
sudo apt update
```
```
exit
```

![](https://lh7-us.googleusercontent.com/WgvldPgx5jL8MoQYkpm47qIuFhGa68GV1gHiiqnLrveV2HX8TRgJhAGH01_7mNeLjOB3vYmHcfK1Ln39xDK7Qjmd0rtRfwGehc1x5TJddX1sRbJLvWXt3NMrJ-Ke_6OOkWa_FknLwd_xBhNmY1wHioY)

**17. Modify the user account "john_doe" to change the default shell to "/bin/bash" and set the account's expiration date to one month from today.**
```
sudo chsh -s /bin/bash john_doe
```
```
sudo chage -E $(date -d "+1 month" +"%Y-%m-%d") john_doe
```
```
sudo chage -l john_doe
```
```
grep john_doe /etc/passwd
```

![](https://lh7-us.googleusercontent.com/ltw7Zq8hKEMirYUFT2vajU-n87fVGhszLKqsATPek-WvuvRhwR8jo32n2gxhuGdGZZn5f5Tz-WRBgw85mxvEg6M3WViOD30YigI_i5DHSMNpNHUF_isfmdwmQnxpM8sWJoIaL1xleYaL0r4fiM_3Zuw)

**18. Create a new group named "development_team." Add "john_doe" to this group and verify the group's existence.**
```
grep development_team /etc/group
```
```
sudo addgroup development_team
```
```
grep development_team /etc/group
```
```
sudo adduser john_doe development_team
```
```
id john_doe
```

![](https://lh7-us.googleusercontent.com/g7VyJbK91N2RRhJjVIeEynbzIvRXc3EKOXRWPHeSV_Y-GlTT449OlDhmKhjpqBfr7jUMYBPMEq64o1397dDeAa02ZN0W0B-Itm6_vGjipxnHOZMVlyxrOWKCNqKIkKkUZsxt0T3otHQA_72BQ7LkLlE)

**19. Remove "john_doe" from the "users" group and add them to the "development_team" group. Confirm the changes.**
```
id john_doe
```
```
sudo deluser john_doe users
```
```
sudo adduser john_doe development_team
```
```
id john_doe
```

![](https://lh7-us.googleusercontent.com/8wmq_Mj7-Io2SJ0CNG5mbrAcA-1y9lfY1i19XLiFzIyaY7TAmnSN7EHb7SYmsi266cwuPQb4gfzvzpVQ9114fB_hAmR5216gOcUR0kNk9x0eIffRcGQ7VjXsk0I3v_pQ0TbVeZkRH-dXl93gsTlA1Rw)

**20. Delete the user account "john_doe" and ensure that their home directory is also removed.**
```
sudo deluser --remove-home john_doe
```
```
id john_doe
```
```
ls /home/john_doe
```
![](https://lh7-us.googleusercontent.com/JDPgvRDH5M3S4af31v1NowEnR6JbYWZXjH9k-Vx8_mcM4tcfWyEiL2Zz6jeVycxgBwYg1LMCX3fd8WC8GgMwdXEZB-Aj7J2-ekfVuHajHQS2gEpKdJBFzR8QeehQxYBSUWi2iUWNUb92fqoWFUNb9J8)

**21. Delete the group "development_team" and ensure that all users previously belonging to the group are appropriately handled.**
```
sudo deluser john_doe development_team
```
```
sudo delgroup development_team
```
```
grep development_team /etc/group
```

![](https://lh7-us.googleusercontent.com/uVgHPZDsT52dEhjLeap33R5lVMHqtnNe7P2UoDwxa_abYRAgUlx6QdLdA-K6difUM2JItgb558G2bwCGHn2CEsGOcuegBwJ4gMFmEynXpzq5oHIjrsVhHTOQx5CmRXen6KdNoHHdZfK_NQ_8k2HJM3g)

**22. Implement a password policy that requires users to change their passwords every 90 days. Apply this policy to all existing and new user accounts.**
```
sudo chage -M 90 -m 0 -W 7 -I 30 -E -1 $(cut -d: -f1 /etc/passwd)
```
```
sudo sed -i '/PASS_MAX_DAYS/c\PASS_MAX_DAYS   90' /etc/login.defs
```
```
sudo chage -l john_doe
```
```
grep PASS_MAX_DAYS /etc/login.defs
```
![](https://lh7-us.googleusercontent.com/Dzn6MmvFb1yMKvym754fZwr3uRmrhLq-5MWhyYPZD_A1m5lrqk3WTirw9J41WXPMYCpWRzSpYoUxdmQi3dFlNCcTfq_sAJ3qoPJwMUE6iSQS4ImEgbYRmCBp2IdRy2QcZx6Mnp5ZdDKQ4r4Rza6TQRg)

**23. Manually lock the user account "john_doe." Attempt to log in as "john_doe" to confirm that the account is locked. Then, unlock the account.**
```
sudo passwd -l john_doe
```
```
sudo su - john_doe
```
```
exit
```
```
sudo passwd -u john_doe
```
```
su - john_doe
```
![](https://lh7-us.googleusercontent.com/bUuwNF0IUUrDtL4kCfcg4zNbxE3Hp-TYvdsdrsRFSakxJK1El5OGkzPt-iwSNhFy7SNV3dWdLbaaKgIo9Rhi-HYpwmmhVGy5qu8Fm0E5H-XFHD3XsJAmN7wxwhsS_E9YtFPUtEbrA8XHIajc7WCMth4)

**24. Use the id command to display detailed information about the "john_doe" user, including user ID, group ID, and supplementary groups.**
```
id john_doe
```
![](https://lh7-us.googleusercontent.com/ZgRMmZXAQ8QTMIJszCmW91JOj7ET_bZmhivtl-A97ri2HzPtnhLkjLsvgMc--tyHl3eapcVMovSrkoKylgBf20Wuf5azIfemznquPB0m-UmjLlbwhLmcpy4vwMBcRSN5WaufGwF7U2YY6h_onUfTqLE)

**25. Configure the password aging for the user "john_doe" to enforce a maximum password age of 60 days. Confirm that the changes take effect.**
```
sudo grep 'john_doe' /etc/passwd
```
```
sudo chage -M 60 john_doe
```
```
sudo chage -l john_doe
```
![](https://lh7-us.googleusercontent.com/ld5PUlApJPXmQ-4fewFTEDy7XDgcPWBUyiftkKb2oYlVtTt86M7zNlZHGbDPyOoNpZ8beS3ExQg8fMKqBgARQq5brOIHUxAqbwF0f20Gd4T_6FWG3AjTEu5CwhjjiakrszW39JcWj8v1GYtBvQZeKgE)
