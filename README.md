# SimpleDynamo
Implementation of a Dynamo-style key-value storage

### Prerequisite Installations

1. Install Android Studio

2. Configure -> SDK Manager -> Uncheck Android Studio 10.0 (Q) and check Android 4.4 (KitKat) -> Apply changes

3. Show Package Details -> check Google APIs Intel x86 Atom
   System Image - > Apply changes

4. Use Java 8 or lower and make sure the appropriate JDK is used in the studio.

5. Enable [VM acceleration](https://developer.android.com/studio/run/emulator-acceleration.html#accel-vm) .

6. Complete some installations if using [Ubuntu](https://stackoverflow.com/questions/27078052/android-studio-build-error-on-ubuntu-install).

7. Add the following lines to .bash file 

   ```bash
   # Android studio paths
   export ANDROID_HOME=$HOME/Android/Sdk
   export PATH=$PATH:$ANDROID_HOME/tools/bin
   export PATH=$PATH:$ANDROID_HOME/platform-tools
   export PATH=$PATH:$ANDROID_HOME/emulator
   ```



### Creating the AVDs

All the files can be found the test directory.

```bash
# creating AVDs (to be run one time only)
python create_avd.py <numAVDs>
# running the AVDs
python run_avd.py <num_AVDs>
# creating a network to connect the AVDs
python set_redir.py 10000
```





### References

[1] **Project Specification (Use PA 4):** https://cse.buffalo.edu/~stevko/courses/cse486/spring19/pas.html

[2] **Related Paper:** DeCandia, Giuseppe, Deniz Hastorun, Madan Jampani, Gunavardhan Kakulapati, Avinash Lakshman, Alex Pilchin, Swaminathan Sivasubramanian, Peter Vosshall, and Werner Vogels. "Dynamo: Amazon's highly available key-value store." *ACM SIGOPS operating systems review* 41, no. 6 (2007): 205-220.

[2] **Testing code:** Link in Project Specification





