# SWE_2021_41_2024_2_week_6
## Week 4 Assignment

[<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/Github-desktop-logo-symbol.svg/1024px-Github-desktop-logo-symbol.svg.png" width = "80px">](https://github.com/w0uldy0u/SWE_2021_41_2024_2_week_4)

[<b>Week 4 Repository</b>](https://github.com/w0uldy0u/SWE_2021_41_2024_2_week_4)
<br>

```python
def isHappy(n):
  while True:
    temp = 0

    for i in str(n):
      temp += int(i) ** 2

    n = temp

    if n == 4:
      return False
    elif n == 1:
      return True

```

* The `isHappy()` function is used to determine whether the given number `n` is a happy number
* To determine if a number is a happy number, we sum the squares of its digits, which is done by the for loop in the code
* If a number is not a happy number, it will eventually fall into a endless cycle that includes 4
* So if a number becomes 4 at some point, we know it's not a happy number and therefore the function returns `False`
* According to the definition of happy number, if a number becomes 1, it is a happy number so the function returns `True`
<br>
<br>

## Week 5 Assignment
>___Input___
>>The command shows the OS information installed in the Docker container
>```zsh
>docker exec ossp-container cat /etc/os-release
>```
>---
>___Output___
>```zsh
>PRETTY_NAME="Ubuntu 24.04.1 LTS"
>NAME="Ubuntu"
>VERSION_ID="24.04"
>VERSION="24.04.1 LTS (Noble Numbat)"
>VERSION_CODENAME=noble
>ID=ubuntu
>ID_LIKE=debian
>HOME_URL="https://www.ubuntu.com/"
>SUPPORT_URL="https://help.ubuntu.com/"
>BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
>PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
>UBUNTU_CODENAME=noble
>LOGO=ubuntu-logo
>```
<br>
<br>

>___Input___
>>The command shows the version of Git installed in the Docker container
>```zsh
>docker exec ossp-container git --version
>```
>---
>___Output___
>```zsh
>git version 2.43.0
>```
<br>
<br>

>___Input___
>>The command shows the version of Python installed in the Docker container
>```zsh
>docker exec ossp-container python3 --version
>```
>---
>___Output___
>```zsh
>Python 3.12.3
>```
<br>
<br>

>___Input___
>>The command shows the path of mounted directory in the Docker container
>```zsh
>docker inspect --format="{{ .HostConfig.Binds }}" ossp-container
>```
>---
>___Output___
>```zsh
>[/Users/space/Library/CloudStorage/OneDrive-성균관대학교/24-2/Open Source/Docker files:/mnt/ossp_container_dir]
>```
