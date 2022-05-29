# LINUX Commands

---

## Special Characters

| Sr. No. | Character | Description            |
| ------- | --------- | ---------------------- |
| 1       | /         | Root Directory         |
| 2       | ~         | Home directory of user |
| 3       | $         | System user            |
| 4       | #         | Root user              |

---

## Linux top-level Directories

| Sr. No. | Path        | Files Contained                                                               |
| ------- | ----------- | ----------------------------------------------------------------------------- |
| 1       | /           | Single root directory – file system base                                      |
| 2       | /bin        | Executable files such as Linux commands cat,cp,ls                             |
| 3       | /boot       | Files that the boot loaders access during start-up–including the Linux kernel |
| 4       | /dev        | Files for the different hardware/devices                                      |
| 5       | /etc.       | Initialization scripts and system config files                                |
| 6       | /home       | User directories                                                              |
| 7       | /lib        | Library files which includes driver modules                                   |
| 8       | /lost+found | For lost files                                                                |
| 9       | /media      | Mounting removal media filesystems                                            |
| 10      | /mnt        | Temporary directory for mounted filesystems                                   |
| 11      | /opt        | For storing application packages                                              |
| 12      | /proc       | Information on Linux processes                                                |
| 13      | /root       | Root user home directory                                                      |
| 14      | /sbin       | Executable files for commands used by root user                               |
| 15      | /srv        | For services hosted by the system (e.g. FTP, web)                             |
| 16      | /tmp        | Temporary directory – deleted during system reboot                            |
| 17      | /usr        | Contains subdirectories for program files                                     |
| 18      | /var        | Log files                                                                     |

---

## Command Line Shortcuts

| Sr. No. | Shotcut             | Description                                 |
| ------- | ------------------- | ------------------------------------------- |
| 1       | ctrl + alt +t       | Open terminal                               |
| 2       | arrow up and down   | scroll up or down                           |
| 3       | arrow left or right | Move curser left or right                   |
| 4       | tab                 | Auto complete command                       |
| 5       | double tab          | List of all commands linked to some command |
| 6       | ctrl + shift + c    | Copy selected text                          |
| 7       | ctrl + shift + v    | Paste copied data                           |
| 8       | ctrl + a            | Move curser to beginning of line            |
| 9       | ctrl + e            | Move curser to end of line                  |
| 10      | space               | Next page                                   |
| 11      | backspace           | Delete charcter left to curser              |
| 12      | del Key             | Delete charcter under curser                |
| 13      | &                   | Combine two commands                        |
| 14      | ctrl + r            | Seach a command in history                  |
| 15      | ctrl + c            | End running command                         |
| 16      | q                   | Exit from a running command                 |

---

## Commands

### Help commands

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=1>1</td>
      <td rowspan=1>1</td>
      <td rowspan=1>man</td>
      <td rowspan=2>&lt;command&gt;</td>
      <td rowspan=1>Display the user manual of any command that we can run on the terminal (offline)</td>
    </tr>
    <tr>
      <td rowspan=1>2</td>
      <td rowspan=1>2</td>
      <td rowspan=1>whatis</td>
      <td rowspan=1>Get a one-line manual page descriptions</td>
    </tr>
    <tr>
      <td rowspan=1>3</td>
      <td rowspan=1>3</td>
      <td rowspan=1>&lt;command&gt;</td>
      <td rowspan=1>--help</td>
      <td rowspan=1>Short help manul for a command</td>
    </tr>
    <tr>
      <td rowspan=1>4</td>
      <td rowspan=1>4</td>
      <td rowspan=1>info</td>
      <td rowspan=2>&lt;command&gt;</td>
      <td rowspan=1>Reads documentation in the info format (online)</td>
    </tr>
    <tr>
      <td rowspan=1>5</td>
      <td rowspan=1>5</td>
      <td rowspan=1>type</td>
      <td rowspan=1>Find location of command in the system</td>
    </tr>
    <tr>
      <td rowspan=5>6</td>
      <td rowspan=1>6</td>
      <td rowspan=5>alias</td>
      <td rowspan=1></td>
      <td rowspan=2>Display defined aliases</td>
    </tr>
    <tr>
      <td rowspan=1>7</td>
      <td rowspan=1>-p</td>
    </tr>
    <tr>
      <td rowspan=1>8</td>
      <td rowspan=1>&lt;shortcut&gt;=&lt;command&gt;</td>
      <td rowspan=1>Create new alias (shortcut command)</td>
    </tr>
    <tr>
      <td rowspan=1>9</td>
      <td rowspan=1>&lt;shortcut&gt;=-</td>
      <td rowspan=1>Update alias with impractical data</td>
    </tr>
    <tr>
      <td rowspan=1>10</td>
      <td rowspan=1>&lt;shortcut&gt;=</td>
      <td rowspan=1>Remove command from alias</td>
    </tr>
    <tr>
      <td rowspan=1>7</td>
      <td rowspan=1>11</td>
      <td rowspan=1>unalias</td>
      <td rowspan=1>&lt;shortcut&gt;</td>
      <td rowspan=1>Delete alias</td>
    </tr>
  </tbody>
</table>

### General Commands

| Cmd. No. | Sr. No | Command           | Description                        |
| -------- | ------ | ----------------- | ---------------------------------- |
| 1        | 12     | clear             | Clear terminal window              |
| 2        | 13     | history           | List of all coomands used          |
| 3        | 14     | !<command_number> | Execute a command from the history |
| 4        | 15     | date              | Display current date and time      |
| 5        | 16     | cal               | Display calander                   |

### CPU Information

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=2>1</td>
      <td rowspan=1>17</td>
      <td rowspan=2>uptime</td>
      <td rowspan=1></td>
      <td rowspan=1>Display curren time, uptime, no of users and load average</td>
    </tr>
    <tr>
      <td rowspan=1>18</td>
      <td rowspan=1>-p</td>
      <td rowspan=1>Display uptime</td>
    </tr>
    <tr>
      <td rowspan=2>2</td>
      <td rowspan=1>19</td>
      <td rowspan=2>hostname</td>
      <td rowspan=1></td>
      <td rowspan=1>Display hostname</td>
    </tr>
    <tr>
      <td rowspan=1>20</td>
      <td rowspan=1>-i</td>
      <td rowspan=1>Display ip address</td>
    </tr>
    <tr>
      <td rowspan=1>3</td>
      <td rowspan=1>21</td>
      <td rowspan=1>lscpu</td>
      <td rowspan=1></td>
      <td rowspan=1>Display information about the CPU architecture</td>
    </tr>
    <tr>
      <td rowspan=1>4</td>
      <td rowspan=1>22</td>
      <td rowspan=1>cat</td>
      <td rowspan=1>proc/cpuinfo</td>
      <td rowspan=1>CPU detailed info</td>
    </tr>
    <tr>
      <td rowspan=6>5</td>
      <td rowspan=1>23</td>
      <td rowspan=6>uanme</td>
      <td rowspan=1></td>
      <td rowspan=1>Print system information</td>
    </tr>
    <tr>
      <td rowspan=1>24</td>
      <td rowspan=1>-a</td>
      <td rowspan=1>Print all information (machine, processer and OS)</td>
    </tr>
    <tr>
      <td rowspan=1>25</td>
      <td rowspan=1>-s</td>
      <td rowspan=1>Print the operating system name</td>
    </tr>
    <tr>
      <td rowspan=1>26</td>
      <td rowspan=1>-r</td>
      <td rowspan=1>Print the operating system release</td>
    </tr>
    <tr>
      <td rowspan=1>27</td>
      <td rowspan=1>-v</td>
      <td rowspan=1>Print the operating system version</td>
    </tr>
    <tr>
      <td rowspan=1>28</td>
      <td rowspan=1>-p</td>
      <td rowspan=1>Print the processer type</td>
    </tr>
    <tr>
      <td rowspan=1>6</td>
      <td rowspan=1>29</td>
      <td rowspan=1>ifconfig</td>
      <td rowspan=1></td>
      <td rowspan=1>Configure the kernel-resident network interfaces (package)</td>
    </tr>
    <tr>
      <td rowspan=1>7</td>
      <td rowspan=1>30</td>
      <td rowspan=1>cupid</td>
      <td rowspan=1></td>
      <td rowspan=1>Tool to dump x86 CPUID information about the CPU (package)</td>
    </tr>
  </tbody>
</table>

### Disk Information

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Argument 2</th>
      <th>Argument 3</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=2>1</td>
      <td rowspan=1>31</td>
      <td rowspan=2>df</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Get a full summary of available and used disk space usage of the file system.</td>
    </tr>
    <tr>
      <td rowspan=1>32</td>
      <td rowspan=1>-h</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Get a full summary of available and used disk space usage of the file system (human readable form)</td>
    </tr>
    <tr>
      <td rowspan=4>2</td>
      <td rowspan=1>33</td>
      <td rowspan=4>du</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Check the information of disk usage of files and directories on a machine</td>
    </tr>
    <tr>
      <td rowspan=1>34</td>
      <td rowspan=1>-h</td>
      <td rowspan=1>|</td>
      <td rowspan=1>less</td>
      <td rowspan=1>Check the information of disk usage of files and directories on a machine (human readable page by page)</td>
    </tr>
    <tr>
      <td rowspan=1>35</td>
      <td rowspan=2>&lt;directory_path&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Check the information of disk usage of directories for a specific path</td>
    </tr>
    <tr>
      <td rowspan=1>36</td>
      <td rowspan=1>-s</td>
      <td rowspan=1></td>
      <td rowspan=1>Check the information of disk usage of directory</td>
    </tr>
  </tbody>
</table>

### Managing Processes

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Argument 2</th>
      <th>Argument 3</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=2>1</td>
      <td rowspan=1>37</td>
      <td rowspan=2>free</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Display amount of free and used memory in the system</td>
    </tr>
    <tr>
      <td rowspan=1>38</td>
      <td rowspan=1>-h</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Display amount of free and used memory in the system (human readable)</td>
    </tr>
    <tr>
      <td rowspan=1>2</td>
      <td rowspan=1>39</td>
      <td rowspan=1>top</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Show the Linux processes</td>
    </tr>
    <tr>
      <td rowspan=4>3</td>
      <td rowspan=1>40</td>
      <td rowspan=4>ps</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Snapshot of current processes</td>
    </tr>
    <tr>
      <td rowspan=1>41</td>
      <td rowspan=1>-a</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>All processes except session leaders and processes not associated with a terminal</td>
    </tr>
    <tr>
      <td rowspan=1>42</td>
      <td rowspan=2>-aux</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Show every process on the system</td>
    </tr>
    <tr>
      <td rowspan=1>43</td>
      <td rowspan=1>| grep</td>
      <td rowspan=1>&lt;search_string&gt;</td>
      <td rowspan=1>Show every process on the system including search string</td>
    </tr>
    <tr>
      <td rowspan=1>4</td>
      <td rowspan=1>44</td>
      <td rowspan=1>kill</td>
      <td rowspan=1>&lt;process_id&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Kill a process</td>
    </tr>
    <tr>
      <td rowspan=2>5</td>
      <td rowspan=1>45</td>
      <td rowspan=2>nice</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List low priority program</td>
    </tr>
    <tr>
      <td rowspan=1>46</td>
      <td rowspan=1>-n</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Set priority to a program</td>
    </tr>
    <tr>
      <td rowspan=2>6</td>
      <td rowspan=1>47</td>
      <td rowspan=2>bg</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List all background processes</td>
    </tr>
    <tr>
      <td rowspan=1>48</td>
      <td rowspan=1>&lt;command&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Run a process in background</td>
    </tr>
    <tr>
      <td rowspan=2>7</td>
      <td rowspan=1>49</td>
      <td rowspan=2>reboot</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Restart system</td>
    </tr>
    <tr>
      <td rowspan=1>50</td>
      <td rowspan=1>-p</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=2>Turn off system</td>
    </tr>
    <tr>
      <td rowspan=2>8</td>
      <td rowspan=1>51</td>
      <td rowspan=2>shutdown</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
    </tr>
    <tr>
      <td rowspan=1>52</td>
      <td rowspan=1>-r</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Restart system</td>
    </tr>
  </tbody>
</table>

### Package Managemant

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Argument 2</th>
      <th>Argument 3</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=1>1</td>
      <td rowspan=1>53</td>
      <td rowspan=1>apt-cache</td>
      <td rowspan=1>search</td>
      <td rowspan=1>&lt;keyword&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Display all packages available against a keyword</td>
    </tr>
    <tr>
      <td rowspan=3>2</td>
      <td rowspan=1>54</td>
      <td rowspan=3>apt-get</td>
      <td rowspan=1>update</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Fetch updated packages from source</td>
    </tr>
    <tr>
      <td rowspan=1>55</td>
      <td rowspan=1>upgrade</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Install updated packages</td>
    </tr>
    <tr>
      <td rowspan=1>56</td>
      <td rowspan=2>install</td>
      <td rowspan=4>&lt;package_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=2>Install a package</td>
    </tr>
    <tr>
      <td rowspan=4>3</td>
      <td rowspan=1>57</td>
      <td rowspan=4>apt</td>
      <td rowspan=1></td>
    </tr>
    <tr>
      <td rowspan=1>58</td>
      <td rowspan=2>remove</td>
      <td rowspan=1></td>
      <td rowspan=1>Remove package</td>
    </tr>
    <tr>
      <td rowspan=1>59</td>
      <td rowspan=1>--purge</td>
      <td rowspan=1>Remove package along with configration files</td>
    </tr>
    <tr>
      <td rowspan=1>60</td>
      <td rowspan=1>list</td>
      <td rowspan=1>--installed</td>
      <td rowspan=1></td>
      <td rowspan=1>List all installed packages</td>
    </tr>
  </tbody>
</table>

### User and Security Management

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Argument 2</th>
      <th>Argument 3</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=1>1</td>
      <td rowspan=1>61</td>
      <td rowspan=1>w</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Find who is online</td>
    </tr>
    <tr>
      <td rowspan=2>2</td>
      <td rowspan=1>62</td>
      <td rowspan=2>sudo</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Gain all access for normal user</td>
    </tr>
    <tr>
      <td rowspan=1>63</td>
      <td rowspan=1>su</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=3>Switch to root user in current working directory</td>
    </tr>
    <tr>
      <td rowspan=4>3</td>
      <td rowspan=1>64</td>
      <td rowspan=4>su</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
    </tr>
    <tr>
      <td rowspan=1>65</td>
      <td rowspan=1>root</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
    </tr>
    <tr>
      <td rowspan=1>66</td>
      <td rowspan=1>-</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Switch to root user</td>
    </tr>
    <tr>
      <td rowspan=1>67</td>
      <td rowspan=1>&lt;user_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Switch to user</td>
    </tr>
    <tr>
      <td rowspan=1>4</td>
      <td rowspan=1>68</td>
      <td rowspan=1>exit</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Exit root user</td>
    </tr>
    <tr>
      <td rowspan=2>5</td>
      <td rowspan=1>69</td>
      <td rowspan=2>useradd</td>
      <td rowspan=4>&lt;user_name&gt;</td>
      <td rowspan=1>-c</td>
      <td rowspan=1>&lt;Description&gt;</td>
      <td rowspan=1>Create user with short description (full name)</td>
    </tr>
    <tr>
      <td rowspan=1>70</td>
      <td rowspan=1>-m</td>
      <td rowspan=1></td>
      <td rowspan=1>Create user along with home directory</td>
    </tr>
    <tr>
      <td rowspan=1>6</td>
      <td rowspan=1>71</td>
      <td rowspan=1>userdel</td>
      <td rowspan=1>-r</td>
      <td rowspan=1></td>
      <td rowspan=1>Delet user </td>
    </tr>
    <tr>
      <td rowspan=1>7</td>
      <td rowspan=1>72</td>
      <td rowspan=1>passwd</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Change password of a user</td>
    </tr>
    <tr>
      <td rowspan=1>8</td>
      <td rowspan=1>73</td>
      <td rowspan=1>cat</td>
      <td rowspan=1>/etc/passwd</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List all users with some extra details</td>
    </tr>
    <tr>
      <td rowspan=1>9</td>
      <td rowspan=1>74</td>
      <td rowspan=1>groupadd</td>
      <td rowspan=1>&lt;group_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Create group</td>
    </tr>
    <tr>
      <td rowspan=1>10</td>
      <td rowspan=1>75</td>
      <td rowspan=1>groups</td>
      <td rowspan=1>&lt;user_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Check groups for user</td>
    </tr>
    <tr>
      <td rowspan=1>11</td>
      <td rowspan=1>76</td>
      <td rowspan=1>usermod</td>
      <td rowspan=1>-aG</td>
      <td rowspan=1>&lt;group_name&gt;</td>
      <td rowspan=1>&lt;user_name&gt;</td>
      <td rowspan=1>Add user to group</td>
    </tr>
    <tr>
      <td rowspan=1>12</td>
      <td rowspan=1>77</td>
      <td rowspan=1>groupdel</td>
      <td rowspan=1>&lt;group_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Delete group</td>
    </tr>
    <tr>
      <td rowspan=1>13</td>
      <td rowspan=1>78</td>
      <td rowspan=1>cat</td>
      <td rowspan=1>/etc/group</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List all groups with details</td>
    </tr>
    <tr>
      <td rowspan=1>14</td>
      <td rowspan=1>79</td>
      <td rowspan=1>chown</td>
      <td rowspan=1>&lt;user_name&gt;</td>
      <td rowspan=4>&lt;file_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>changer ownership of a file or directory</td>
    </tr>
    <tr>
      <td rowspan=1>15</td>
      <td rowspan=1>80</td>
      <td rowspan=1>chgrp</td>
      <td rowspan=1>&lt;group_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>changer group of a file or directory</td>
    </tr>
    <tr>
      <td rowspan=2>16</td>
      <td rowspan=1>81</td>
      <td rowspan=2>chmod</td>
      <td rowspan=2>&lt;code&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>grant or revoke permissions</td>
    </tr>
    <tr>
      <td rowspan=1>82</td>
      <td rowspan=1>-R</td>
      <td rowspan=1>grant or revoke permissions (recursive)</td>
    </tr>
  </tbody>
</table>

#### SUDO permission Codes

| Sr.No. | Code | Permission    |
| ------ | ---- | ------------- |
| 1      | 0    | No permission |
| 2      | 1    | executable    |
| 3      | 2    | write         |
| 4      | 4    | read          |
| 5      | x    | executable    |
| 6      | r    | write         |
| 7      | w    | read          |

### Managing Files and Directories

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Argument 2</th>
      <th>Argument 3</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=4>1</td>
      <td rowspan=1>83</td>
      <td rowspan=4>cd</td>
      <td rowspan=1>&lt;directory_path&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Changes directory and goes to dir_path directory</td>
    </tr>
    <tr>
      <td rowspan=1>84</td>
      <td rowspan=1>~</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>The tilde (~) sign signifies the user’s home dir – change dir to home directory</td>
    </tr>
    <tr>
      <td rowspan=1>85</td>
      <td rowspan=1>/</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Move to root</td>
    </tr>
    <tr>
      <td rowspan=1>86</td>
      <td rowspan=1>..</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Means to change directory one level up</td>
    </tr>
    <tr>
      <td rowspan=6>2</td>
      <td rowspan=1>87</td>
      <td rowspan=6>ls</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List down all the contents of a directory</td>
    </tr>
    <tr>
      <td rowspan=1>88</td>
      <td rowspan=1>-a</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List down all the contents of a directory along with hiden files</td>
    </tr>
    <tr>
      <td rowspan=1>89</td>
      <td rowspan=1>&lt;string&gt;*</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List down all the contents of a directory starting with string</td>
    </tr>
    <tr>
      <td rowspan=1>90</td>
      <td rowspan=1>*&lt;string&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List down all the contents of a directory ending with string</td>
    </tr>
    <tr>
      <td rowspan=1>91</td>
      <td rowspan=1>-1 |</td>
      <td rowspan=1>wc -l</td>
      <td rowspan=1></td>
      <td rowspan=1>List number of files in a directory</td>
    </tr>
    <tr>
      <td rowspan=1>92</td>
      <td rowspan=1>-l</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List down all the contents of a directory along with extra information</td>
    </tr>
    <tr>
      <td rowspan=1>3</td>
      <td rowspan=1>93</td>
      <td rowspan=1>mkdir</td>
      <td rowspan=1>&lt;directory_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Create directory</td>
    </tr>
    <tr>
      <td rowspan=1>4</td>
      <td rowspan=1>94</td>
      <td rowspan=1>touch</td>
      <td rowspan=1>&lt;file_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Create a file</td>
    </tr>
    <tr>
      <td rowspan=4>5</td>
      <td rowspan=1>95</td>
      <td rowspan=4>echo</td>
      <td rowspan=1>$SHELL</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Display shell path</td>
    </tr>
    <tr>
      <td rowspan=1>96</td>
      <td rowspan=3>&lt;content&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Disply contnet on terminal</td>
    </tr>
    <tr>
      <td rowspan=1>97</td>
      <td rowspan=1>></td>
      <td rowspan=2>&lt;file_name&gt;</td>
      <td rowspan=1>Create file and write data</td>
    </tr>
    <tr>
      <td rowspan=1>98</td>
      <td rowspan=1>>></td>
      <td rowspan=1>Append data to the file</td>
    </tr>
    <tr>
      <td rowspan=2>6</td>
      <td rowspan=1>99</td>
      <td rowspan=2>cp</td>
      <td rowspan=1>&lt;file_name&gt;</td>
      <td rowspan=1>&lt;directory_path&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Copy file to path</td>
    </tr>
    <tr>
      <td rowspan=1>100</td>
      <td rowspan=1>&lt;directory_path_1&gt;</td>
      <td rowspan=1>&lt;directory_path_2&gt;</td>
      <td rowspan=1>-r</td>
      <td rowspan=1>Copy one directory to other</td>
    </tr>
    <tr>
      <td rowspan=2>7</td>
      <td rowspan=1>101</td>
      <td rowspan=2>mv</td>
      <td rowspan=1>&lt;file_name&gt;</td>
      <td rowspan=1>&lt;directory_path&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Move file to path</td>
    </tr>
    <tr>
      <td rowspan=1>102</td>
      <td rowspan=1>&lt;directory_path_1&gt;</td>
      <td rowspan=1>&lt;directory_path_2&gt;</td>
      <td rowspan=1>-r</td>
      <td rowspan=1>Move one directory to other</td>
    </tr>
    <tr>
      <td rowspan=3>8</td>
      <td rowspan=1>103</td>
      <td rowspan=3>rm</td>
      <td rowspan=1>&lt;file_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Delete a file</td>
    </tr>
    <tr>
      <td rowspan=1>104</td>
      <td rowspan=2>-rf</td>
      <td rowspan=1>&lt;directory_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Delete a folder with mulitple file sin it</td>
    </tr>
    <tr>
      <td rowspan=1>105</td>
      <td rowspan=1>/</td>
      <td rowspan=1></td>
      <td rowspan=1>Delete ubuntu</td>
    </tr>
    <tr>
      <td rowspan=1>9</td>
      <td rowspan=1>106</td>
      <td rowspan=1>rmdir</td>
      <td rowspan=1>&lt;directory_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Delete folder</td>
    </tr>
    <tr>
      <td rowspan=1>10</td>
      <td rowspan=1>107</td>
      <td rowspan=1>wget</td>
      <td rowspan=1>&lt;URL&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Download and save a url page</td>
    </tr>
  </tbody>
</table>

### Processing Files

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Argument 2</th>
      <th>Argument 3</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=1>1</td>
      <td rowspan=1>108</td>
      <td rowspan=1>pwd</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Display the current directory</td>
    </tr>
    <tr>
      <td rowspan=2>2</td>
      <td rowspan=1>109</td>
      <td rowspan=2>cat</td>
      <td rowspan=1>&lt;file_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Print all the contents of file in the terminal</td>
    </tr>
    <tr>
      <td rowspan=1>110</td>
      <td rowspan=1>&lt;multiple_file_names&gt;</td>
      <td rowspan=1>></td>
      <td rowspan=1>&lt;target_file_name&gt;</td>
      <td rowspan=1>merge files</td>
    </tr>
    <tr>
      <td rowspan=1>3</td>
      <td rowspan=1>111</td>
      <td rowspan=1>more</td>
      <td rowspan=8>&lt;file_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Show a text file one page at a time – display can only go forward</td>
    </tr>
    <tr>
      <td rowspan=1>4</td>
      <td rowspan=1>112</td>
      <td rowspan=1>less</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Show a text file one page at a time – display can go forward and backwards</td>
    </tr>
    <tr>
      <td rowspan=1>5</td>
      <td rowspan=1>113</td>
      <td rowspan=1>wc</td>
      <td rowspan=1>-mwl</td>
      <td rowspan=1></td>
      <td rowspan=1>Display the count of the number of characters, words, and lines in a file</td>
    </tr>
    <tr>
      <td rowspan=2>6</td>
      <td rowspan=1>114</td>
      <td rowspan=2>diff</td>
      <td rowspan=2>&lt;file_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Comapre two files and list differences</td>
    </tr>
    <tr>
      <td rowspan=1>115</td>
      <td rowspan=1>-y</td>
      <td rowspan=1>Comapre two files and list differences side by side</td>
    </tr>
    <tr>
      <td rowspan=2>7</td>
      <td rowspan=1>116</td>
      <td rowspan=2>sort</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Arrange the lines in a file in alphabetic order</td>
    </tr>
    <tr>
      <td rowspan=1>117</td>
      <td rowspan=1>-r</td>
      <td rowspan=1></td>
      <td rowspan=1>Arrange the lines in a file in reverse order</td>
    </tr>
    <tr>
      <td rowspan=1>8</td>
      <td rowspan=1>118</td>
      <td rowspan=1>uniq</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Keep unique lines in a file and delete duplicates</td>
    </tr>
    <tr>
      <td rowspan=1>9</td>
      <td rowspan=1>119</td>
      <td rowspan=1>ln</td>
      <td rowspan=1>-s</td>
      <td rowspan=1>&lt;source_file_path&gt;</td>
      <td rowspan=1>&lt;target_file_path&gt;</td>
      <td rowspan=1>Link two files (soft link)</td>
    </tr>
    <tr>
      <td rowspan=1>10</td>
      <td rowspan=1>120</td>
      <td rowspan=1>split</td>
      <td rowspan=1>&lt;number_of_files&gt;</td>
      <td rowspan=2>&lt;file_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Specify a size to break a file into</td>
    </tr>
    <tr>
      <td rowspan=1>11</td>
      <td rowspan=1>121</td>
      <td rowspan=1>grep</td>
      <td rowspan=1>-i</td>
      <td rowspan=1>&lt;expression&gt;</td>
      <td rowspan=1>Display results of finding expressions in a file</td>
    </tr>
    <tr>
      <td rowspan=1>12</td>
      <td rowspan=1>122</td>
      <td rowspan=1>dd</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>copy lines of data and perform different operations</td>
    </tr>
    <tr>
      <td rowspan=1>13</td>
      <td rowspan=1>123</td>
      <td rowspan=1>cut</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Get sections of text in a file</td>
    </tr>
    <tr>
      <td rowspan=2>14</td>
      <td rowspan=1>124</td>
      <td rowspan=2>sed</td>
      <td rowspan=2>s/expression/expression/g</td>
      <td rowspan=2>&lt;file_name&gt;</td>
      <td rowspan=1>&lt;file_name&gt;</td>
      <td rowspan=1>Perform editing commands, then copy to a standard output</td>
    </tr>
    <tr>
      <td rowspan=1>125</td>
      <td rowspan=1>-i</td>
      <td rowspan=1>update same file</td>
    </tr>
  </tbody>
</table>

### Finding Files

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Argument 2</th>
      <th>Argument 3</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=1>1</td>
      <td rowspan=1>126</td>
      <td rowspan=1>which</td>
      <td rowspan=2>&lt;command&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Locate a command</td>
    </tr>
    <tr>
      <td rowspan=1>2</td>
      <td rowspan=1>127</td>
      <td rowspan=1>whereis</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Locate all details about a command</td>
    </tr>
    <tr>
      <td rowspan=3>3</td>
      <td rowspan=1>128</td>
      <td rowspan=3>find</td>
      <td rowspan=3>&lt;directory_path&gt;</td>
      <td rowspan=3>-name</td>
      <td rowspan=1>&lt;file_name&gt;</td>
      <td rowspan=1>Search a file in a directory</td>
    </tr>
    <tr>
      <td rowspan=1>129</td>
      <td rowspan=1>&lt;string&gt;*</td>
      <td rowspan=1>Search all the files starting with string</td>
    </tr>
    <tr>
      <td rowspan=1>130</td>
      <td rowspan=1>*&lt;string&gt;</td>
      <td rowspan=1>Search all the files ending with string</td>
    </tr>
  </tbody>
</table>

### Compressing Files

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Argument 2</th>
      <th>Argument 3</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=1>1</td>
      <td rowspan=1>131</td>
      <td rowspan=1>gzip</td>
      <td rowspan=4>&lt;file_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Compress files with GNU Zip</td>
    </tr>
    <tr>
      <td rowspan=1>2</td>
      <td rowspan=1>132</td>
      <td rowspan=1>gunzip</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Use GNU Zip to decompress files</td>
    </tr>
    <tr>
      <td rowspan=1>3</td>
      <td rowspan=1>133</td>
      <td rowspan=1>compress</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Use to compress a file</td>
    </tr>
    <tr>
      <td rowspan=1>4</td>
      <td rowspan=1>134</td>
      <td rowspan=1>uncompress</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Uncompress files compressed with compress command</td>
    </tr>
    <tr>
      <td rowspan=2>5</td>
      <td rowspan=1>135</td>
      <td rowspan=2>tar</td>
      <td rowspan=1>-cf</td>
      <td rowspan=2>&lt;target_file&gt;</td>
      <td rowspan=1>&lt;files&gt;</td>
      <td rowspan=1>Archive files with one or more directories</td>
    </tr>
    <tr>
      <td rowspan=1>136</td>
      <td rowspan=1>-xf</td>
      <td rowspan=1></td>
      <td rowspan=1>Extract files</td>
    </tr>
  </tbody>
</table>

### Edit Files

<table>
  <thead>
    <tr>
      <th>Cmd. No.</th>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument 1</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=1>1</td>
      <td rowspan=1>137</td>
      <td rowspan=1>nano</td>
      <td rowspan=3>&lt;file_name&gt;</td>
      <td rowspan=1>Open file with nano editor</td>
    </tr>
    <tr>
      <td rowspan=1>2</td>
      <td rowspan=1>138</td>
      <td rowspan=1>gedit</td>
      <td rowspan=1>Open file with GUI editor</td>
    </tr>
    <tr>
      <td rowspan=1>3</td>
      <td rowspan=1>139</td>
      <td rowspan=1>vi</td>
      <td rowspan=1>Open file with VIM editor</td>
    </tr>
  </tbody>
</table>

#### Vim editor commands and shortcuts

| Sr.NO. | Command     | Description                       |
| ------ | ----------- | --------------------------------- |
| 1      | i           | swith to insert mode              |
| 2      | esc         | swith to command mode             |
| 3      | arrows      | getting around                    |
| 4      | o           | newline and insert data           |
| 5      | :q!         | quit without saving               |
| 6      | u           | undo changes                      |
| 7      | /expression | search for expression in the file |
| 8      | gg          | go to first line                  |
| 9      | G           | go to last line                   |
| 10     | nG          | go to n line                      |
| 11     | :w          | write                             |
| 12     | :q          | quit                              |
| 13     | :x          | write and quit                    |
| 14     | :wq         | write and quit                    |
| 15     | shift + zz  | write and quit                    |
