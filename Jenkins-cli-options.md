**BUILD_NUMBER**

The current build number, such as "153"

**BUILD_ID**

The current build id, such as "2005-08-22_23-59-59" (YYYY-MM-DD_hh-mm-ss)

**BUILD_DISPLAY_NAME**

The display name of the current build, which is something like "#153" by default.

**JOB_NAME**

Name of the project of this build, such as "foo" or "foo/bar". (To strip off folder paths from a Bourne shell script, try: ${JOB_NAME##*/})

**BUILD_TAG**

String of "jenkins-${JOB_NAME}-${BUILD_NUMBER}". Convenient to put into a resource file, a jar file, etc for easier identification.

**EXECUTOR_NUMBER**

The unique number that identifies the current executor (among executors of the same machine) thatâ€™s carrying out this build. This is the number you see in the "build executor status", except that the number starts from 0, not 1.

**NODE_NAME**

Name of the slave if the build is on a slave, or "master" if run on master

**NODE_LABELS**

Whitespace-separated list of labels that the node is assigned.

**WORKSPACE**

The absolute path of the directory assigned to the build as a workspace.

**JENKINS_HOME**

The absolute path of the directory assigned on the master node for Jenkins to store data.

**JENKINS_URL**

Full URL of Jenkins, like http://server:port/jenkins/ (note: only available if Jenkins URL set in system configuration)

**BUILD_URL**

Full URL of this build, like http://server:port/jenkins/job/foo/15/ (Jenkins URL must be set)

**JOB_URL**

Full URL of this job, like http://server:port/jenkins/job/foo/ (Jenkins URL must be set)

**SVN_REVISION**

Subversion revision number that's currently checked out to the workspace, such as "12345"

**SVN_URL**

Subversion URL that's currently checked out to the workspace.
