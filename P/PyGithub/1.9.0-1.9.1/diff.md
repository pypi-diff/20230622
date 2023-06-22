# Comparing `tmp/PyGithub-1.9.0.tar.gz` & `tmp/PyGithub-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyGithub-1.9.0.tar", last modified: Mon Nov 19 20:46:41 2012, max compression
+gzip compressed data, was "dist/PyGithub-1.9.1.tar", last modified: Tue Nov 20 18:36:28 2012, max compression
```

## Comparing `PyGithub-1.9.0.tar` & `PyGithub-1.9.1.tar`

### file list

```diff
@@ -1,411 +1,419 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-19 20:46:41.000000 PyGithub-1.9.0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1309 2012-11-19 20:46:41.000000 PyGithub-1.9.0/PKG-INFO
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     3259 2012-11-19 20:41:48.000000 PyGithub-1.9.0/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-19 20:46:41.000000 PyGithub-1.9.0/github/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1692 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/AuthorizationApplication.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2407 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GithubObject.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1717 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Branch.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2324 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GitTree.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      996 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/InputFileContent.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3259 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GistHistoryState.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4013 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Event.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    27119 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/AuthenticatedUser.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2858 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GitBlob.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3930 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/IssueComment.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2409 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Plan.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2725 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GistFile.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3445 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GitTag.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6327 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Authorization.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    15913 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/NamedUser.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6164 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/PullRequestComment.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4147 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/File.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7384 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Commit.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4236 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GitCommit.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3326 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/ContentFile.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2861 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GitRef.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3921 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/RepositoryKey.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2922 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GitTreeElement.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2816 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/PullRequestPart.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6492 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Hook.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5309 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Github.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5929 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/CommitComment.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1471 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/InputGitTreeElement.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2510 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Tag.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1116 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/InputGitAuthor.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6424 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Comparison.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4052 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/PaginatedList.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1197 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     9358 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Download.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2009 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/CommitStats.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2750 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Label.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1030 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GithubException.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1971 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GitAuthor.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3664 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/CommitStatus.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6323 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Team.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    20127 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Organization.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-19 20:46:41.000000 PyGithub-1.9.0/github/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1882 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/IntegrationTest.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1184 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Branch.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2293 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/GitTree.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4376 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Exceptions.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2827 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Issue50.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5235 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Event.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    12644 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/AuthenticatedUser.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1784 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/GitBlob.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1854 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/IssueComment.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1339 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Issue54.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/GitTag.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1902 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Issue80.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1839 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Authentication.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1795 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Issue87.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2767 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Authorization.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     9175 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/NamedUser.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2132 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/PullRequestComment.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1873 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/AllTests.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4940 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Commit.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1089 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/__main__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2218 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/GitCommit.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2851 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Enterprise.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1474 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ContentFile.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-19 20:46:41.000000 PyGithub-1.9.0/github/tests/ReplayData/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      851 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testGetLabel.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    36363 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetSubscriptions.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1926 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateRepositoryWithAutoInit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2278 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testGetComments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2892 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/IssueEvent.testAttributes.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1555 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue87.testCreateIssueWithEscapedPercentInBody.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      937 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/UserKey.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    29397 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetIssues.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      386 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/CommitComment.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1416 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/RepositoryKey.testEdit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    14718 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testFollowing.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42445 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testSearchRepos.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1552 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testEditWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      590 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetTeams.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1023 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testAttributesOfOtherUser.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      741 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Markdown.testRenderGithubFlavoredMarkdown.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    43661 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetIssues.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Gist.testGetComments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1240 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/CommitComment.testEdit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3994 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue80.testIgnoreHttpsFromGithubEnterprise.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    43044 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testWatching.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    19647 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Enterprise.testLongUrl.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6904 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testAssignees.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   621062 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testIntIndexingAfterIteration.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      375 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/GistComment.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      392 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/IssueComment.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   621062 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testIteration.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    21652 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testCreateComment.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   160299 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testInterruptedIterationInSlice.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1591 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateRepository.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    31223 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1039 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/IssueComment.testEdit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4870 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetWatchers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2471 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testMergeWithoutMessage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      476 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetLanguages.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2184 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitCommit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      391 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequestComment.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      711 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Milestone.testGetLabels.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      973 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/UserKey.testEditWithoutArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2239 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTreeWithBaseTree.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1018 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateAuthorizationWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   205049 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testSliceIndexingUntilFourthPage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1966 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Gist.testStarring.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      628 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testMergeWithConflict.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3087 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Markdown.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   159594 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testIntIndexingInThirdPage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1230 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Authentication.testBasicAuthentication.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3461 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Hook.testEditWithAllParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1055 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Gist.testCreateComment.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2495 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testEditResetAssignee.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      950 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetKeys.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1468 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequestComment.testEdit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    14863 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/ContentFile.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      363 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/UserKey.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    39504 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetWatched.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    80097 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetReceivedEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      579 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testMergeWithNothingToDo.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      913 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testSearchUserByEmail.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6099 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testAddAndRemoveLabels.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1508 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateCommentOnFilePosition.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2548 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testCreateIssueWithLabel.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2812 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateRepoWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    61350 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchReposWithLanguage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    41736 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testSearchUsers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5495 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1468 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateKey.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      367 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Authorization.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1928 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testEditWithDefaultBranch.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2377 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitCommitWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      708 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetLabel.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    18227 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchUsersExplicitPagination.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1622 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testEditWithoutArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    43375 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetStarred.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4634 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/IssueEvent.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1230 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1140 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetLabels.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11951 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetReposWithType.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3301 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Label.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6463 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/IssueComment.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3731 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/GitTag.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1682 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Exceptions.testUnknownObject.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6721 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Commit.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1299 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateStatusWithoutOptionalParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      696 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetOrgs.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    44953 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetNetworkEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8260 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Gist.testFork.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    49600 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetIssuesWithWildcards.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1090 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTree.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4602 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testGetIssuesWithLabel.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4117 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetGists.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3532 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Hook.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5198 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreatePull.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1186 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testEditWithoutArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2084 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateGist.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1173 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateMilestoneWithMinimalArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1121 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Milestone.testEditWithMinimalParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1394 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetComments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4157 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCollaborators.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1232 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testEditWithoutParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1108 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Authentication.testOAuthAuthentication.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1101 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTreeWithSha.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    14948 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCompare.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5233 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/GitBlob.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    18368 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Enterprise.testHttp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3372 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue87.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   117727 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testGetGists.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      790 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testGetLabels.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2703 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      382 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/RepositoryKey.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     9119 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequestComment.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2129 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testCreateGist.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1328 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetMembers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11972 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetReposWithArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3763 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Milestone.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      739 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetHooks.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1001 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Authentication.testNoAuthentication.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    36119 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Branch.testCommitCommentsOnLine.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1295 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testCreateIssueComment.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    41736 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchUsers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2671 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateTeamWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1230 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/RateLimiting.testRateLimiting.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4020 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetSubscribers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1660 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testRemoveLabelFromIssue.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   173042 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchReposPagination.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      769 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetContributors.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3557 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetTeams.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4819 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Commit.testGetComments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Label.testEdit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1398 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testLegacySearchIssues.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5834 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/GitTree.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   169972 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetFiles.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1338 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Logging.testLoggingWithOAuthAuthentication.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1598 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testGetLabels.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      386 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Download.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2523 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testMergeWithMessage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5842 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1220 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testAttributes.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      359 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Gist.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    57977 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      640 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Team.testEditWithoutArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    41357 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchReposExplicitPagination.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    52738 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testSliceIndexingInFirstPage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      813 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetAuthorizations.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1226 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Milestone.testEditWithAllParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7653 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3471 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testEditWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6437 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Team.testRepos.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4112 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testDeleteAndSetLabels.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1229 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Logging.testLoggingWithBaseUrl.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1150 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2330 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateRepositoryWithAutoInit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    51406 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetContents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1304 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue54.testConversion.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      983 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetGitRefWithIssue102Reverted.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7735 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreatePullFromIssue.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1487 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateKey.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4987 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetCommits.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1559 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue87.testCreateIssueWithEscapedPercentInTitle.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    22660 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetGitTreeWithRecursive.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5911 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateIssueWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1350 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetMilestones.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2034 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testCreateGistWithoutDescription.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3709 2012-11-19 19:56:53.000000 PyGithub-1.9.0/github/tests/ReplayData/Gist.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1301 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateMilestone.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1867 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testAddLabelToIssue.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    45967 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Event.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1397 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/UserKey.testEditWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    56350 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testGetThirdPage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      747 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetPublicMembers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4640 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/GistComment.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      358 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Team.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    22973 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetStargazers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5048 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testEditWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3925 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/CommitComment.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      382 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Hook.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4502 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetPulls.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3609 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3501 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Download.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7512 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetFollowing.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      859 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateAuthorizationWithoutArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1343 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateIssue.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5073 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Tag.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2788 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   621062 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testSeveralIterations.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    34297 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetOrganizationEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   621062 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testSliceIndexingUntilEnd.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2741 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetRepos.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      983 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetGitRef.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3555 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/GitRef.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1939 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testEditResetMilestone.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1586 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetForks.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1460 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Logging.testLoggingWithBasicAuthentication.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      712 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateTeam.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1562 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testEditWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4289 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetFollowers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1400 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testGetEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5100 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitCommitWithParents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      764 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Authorization.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    60390 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetIssuesWithArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5245 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testEditWithAllParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      382 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Milestone.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      818 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitBlob.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      676 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Team.testEditWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      990 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/RepositoryKey.testEditWithoutParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4019 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue80.testIgnoreHttpsFromGithubEnterpriseWithPort.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    18368 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Enterprise.testSpecificPort.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4928 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetGists.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1825 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateRepositoryWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      884 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/GitRef.testEdit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4755 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetComments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1218 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetIssueComments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      899 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/GitRef.testEditWithForce.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4898 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Team.testMembers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)  1303294 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue33.testClosedIssues.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      725 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetDownloads.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3888 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/Authentication.testSecretKeyAuthentication.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2226 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testMembers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   630715 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue33.testOpenIssues.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2030 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateRepoWithMinimalArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4229 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Authorization.testEdit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1856 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateDownloadWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2743 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetMilestonesWithArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    75894 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1496 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateCommentOnFileLine.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1355 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTagWithAllArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3342 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Gist.testEditWithAllParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3744 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/RepositoryKey.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      848 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Hook.testEditWithMinimalParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3293 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testSetIssueLabels.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    44154 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchRepos.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2744 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetReposWithType.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1248 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTag.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      391 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Exceptions.testBadAuthentication.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3624 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetGitRefs.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    44751 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetPublicEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1256 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testEditWithoutArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1539 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue87.testCreateIssueWithPercentInTitle.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   138453 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetCommits.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2393 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetKeys.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1002 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/GistComment.testEdit.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6572 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateFork.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1368 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateComment.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1398 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testSearchIssues.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1011 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testIssueGetLabels.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     9358 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/CommitStatus.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Exceptions.testInvalidInput.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1535 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue87.testCreateIssueWithPercentInBody.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      912 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateHookWithMinimalParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1536 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetRepo.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4970 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testEditWithoutArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1128 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue.testCreateComment.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    86542 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetIssuesEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2019 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateGistWithoutDescription.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2460 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetArchiveLink.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      380 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Label.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    18366 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetRepos.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1500 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateStatusWithAllParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    52738 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testGetFirstPage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      947 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue50.testCreateLabel.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    48812 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testStarring.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    17224 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testGetHooks.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    58233 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchUsersPagination.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2703 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue33.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2285 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetBranch.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   160299 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testInterruptedIteration.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1911 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Gist.testEditWithoutParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      686 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetOrgs.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      408 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/GitRef.testDelete.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1744 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateDownloadWithMinimalArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3972 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Branch.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10450 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetPullsWithArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    44947 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      949 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateHookWithAllParameters.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   178014 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequestFile.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6950 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateFork.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1006 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitRef.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8387 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testMergeWithCommitMessage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    80111 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetPublicReceivedEvents.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      385 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Hook.testTest.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    52738 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testIntIndexingInFirstPage.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2300 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetStarredGists.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      676 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Markdown.testRenderMarkdown.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      478 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Exceptions.testUnknownUser.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3100 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Organization.testPublicMembers.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1459 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testMerge.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    44098 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testSubscriptions.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4157 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/GitCommit.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1866 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/ReplayData/Authentication.testUserAgent.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1221 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetIssueComment.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2507 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testEmails.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13052 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetRepos.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    18369 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Enterprise.testHttps.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      877 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateLabel.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10891 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetCommitsWithArguments.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1722 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Team.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1217 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Logging.testLoggingWithoutAuthentication.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3105 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Issue54.setUp.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2280 2012-11-03 09:30:30.000000 PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchUserByEmail.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1795 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/GitRef.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2761 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/RepositoryKey.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2787 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Hook.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2071 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/CommitComment.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7394 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Framework.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1342 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Tag.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4473 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/PaginatedList.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1189 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7545 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Logging_.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2296 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/PullRequestFile.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1244 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Issue33.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2355 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Download.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1594 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Label.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1870 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/CommitStatus.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2930 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Team.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6529 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Organization.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6381 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Gist.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2673 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Milestone.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    30558 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Repository.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    12156 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Github_.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1517 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Markdown.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1040 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/RateLimiting.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6642 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/PullRequest.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1561 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/IssueEvent.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5249 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/Issue.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1810 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/GistComment.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2749 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/tests/UserKey.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1978 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/HookResponse.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10729 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Gist.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7040 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Milestone.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    44921 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Repository.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1923 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GitObject.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2065 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/IssuePullRequest.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1922 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Permissions.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6718 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Requester.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/PullRequestMergeStatus.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    17406 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/PullRequest.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2500 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/HookDescription.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3893 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/IssueEvent.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13410 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Issue.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3929 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/GistComment.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3617 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/UserKey.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6028 2012-11-19 20:40:49.000000 PyGithub-1.9.0/github/Legacy.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-20 18:36:28.000000 PyGithub-1.9.1/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1309 2012-11-20 18:36:28.000000 PyGithub-1.9.1/PKG-INFO
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     3259 2012-11-20 18:36:07.000000 PyGithub-1.9.1/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1692 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/AuthorizationApplication.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2407 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GithubObject.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1717 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Branch.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2324 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GitTree.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7651 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/COPYING.LESSER
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      996 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/InputFileContent.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3259 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GistHistoryState.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4013 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Event.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    27215 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/AuthenticatedUser.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2866 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GitBlob.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3938 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/IssueComment.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2433 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Plan.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2733 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GistFile.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3445 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GitTag.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6335 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Authorization.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    16001 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/NamedUser.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6188 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/PullRequestComment.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4171 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/File.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7400 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Commit.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4236 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GitCommit.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3334 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/ContentFile.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2861 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GitRef.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3929 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/RepositoryKey.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2930 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GitTreeElement.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2816 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/PullRequestPart.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6500 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Hook.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5309 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Github.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5953 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/CommitComment.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1471 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/InputGitTreeElement.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2510 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Tag.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1116 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/InputGitAuthor.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6448 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Comparison.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4060 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/PaginatedList.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1197 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     9382 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Download.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2033 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/CommitStats.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2750 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Label.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1030 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GithubException.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1971 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GitAuthor.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3672 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/CommitStatus.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6347 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Team.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    35147 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/COPYING
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    20215 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Organization.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/doc/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10083 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/doc/ChangeLog.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    15650 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/doc/ReferenceOfApis.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1832 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/doc/Design.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    31883 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/doc/ReferenceOfClasses.md
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1882 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/IntegrationTest.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1184 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Branch.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2293 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/GitTree.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4376 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Exceptions.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2827 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Issue50.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5235 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Event.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    12644 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/AuthenticatedUser.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1784 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/GitBlob.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1854 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/IssueComment.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1339 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Issue54.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/GitTag.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1902 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Issue80.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1839 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Authentication.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1795 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Issue87.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2767 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Authorization.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     9175 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/NamedUser.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2132 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/PullRequestComment.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1873 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/AllTests.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4940 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Commit.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1089 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/__main__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2218 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/GitCommit.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2851 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Enterprise.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1474 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/ContentFile.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/tests/ReplayData/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      851 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testGetLabel.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    36363 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetSubscriptions.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1926 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateRepositoryWithAutoInit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2278 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testGetComments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2892 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/IssueEvent.testAttributes.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1555 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue87.testCreateIssueWithEscapedPercentInBody.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      937 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/UserKey.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    29397 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetIssues.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      386 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/CommitComment.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1416 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/RepositoryKey.testEdit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    14718 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testFollowing.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42445 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testSearchRepos.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1552 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testEditWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      590 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetTeams.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1023 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testAttributesOfOtherUser.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      741 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Markdown.testRenderGithubFlavoredMarkdown.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    43661 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetIssues.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Gist.testGetComments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1240 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/CommitComment.testEdit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3994 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue80.testIgnoreHttpsFromGithubEnterprise.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    43044 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testWatching.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    19647 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Enterprise.testLongUrl.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6904 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testAssignees.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   621062 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testIntIndexingAfterIteration.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      375 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/GistComment.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      392 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/IssueComment.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   621062 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testIteration.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    21652 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testCreateComment.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   160299 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testInterruptedIterationInSlice.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1591 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateRepository.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    31223 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1039 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/IssueComment.testEdit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4870 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetWatchers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2471 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testMergeWithoutMessage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      476 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetLanguages.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2184 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitCommit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      391 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequestComment.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      711 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Milestone.testGetLabels.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      973 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/UserKey.testEditWithoutArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2239 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTreeWithBaseTree.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1018 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateAuthorizationWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   205049 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testSliceIndexingUntilFourthPage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1966 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Gist.testStarring.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      628 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testMergeWithConflict.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3087 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Markdown.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   159594 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testIntIndexingInThirdPage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1230 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Authentication.testBasicAuthentication.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3461 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Hook.testEditWithAllParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1055 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Gist.testCreateComment.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2495 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testEditResetAssignee.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      950 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetKeys.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1468 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequestComment.testEdit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    14863 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/ContentFile.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      363 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/UserKey.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    39504 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetWatched.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    80097 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetReceivedEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      579 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testMergeWithNothingToDo.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      913 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testSearchUserByEmail.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6099 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testAddAndRemoveLabels.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1508 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateCommentOnFilePosition.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2548 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testCreateIssueWithLabel.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2812 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateRepoWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    61350 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchReposWithLanguage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    41736 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testSearchUsers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5495 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1468 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateKey.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      367 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Authorization.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1928 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testEditWithDefaultBranch.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2377 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitCommitWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      708 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetLabel.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    18227 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchUsersExplicitPagination.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1622 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testEditWithoutArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    43375 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetStarred.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4634 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/IssueEvent.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1230 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1140 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetLabels.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11951 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetReposWithType.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3301 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Label.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6463 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/IssueComment.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3731 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/GitTag.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1682 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Exceptions.testUnknownObject.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6721 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Commit.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1299 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateStatusWithoutOptionalParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      696 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetOrgs.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    44953 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetNetworkEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8260 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Gist.testFork.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    49600 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetIssuesWithWildcards.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1090 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTree.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4602 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testGetIssuesWithLabel.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4117 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetGists.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3532 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Hook.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5198 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreatePull.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1186 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testEditWithoutArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2084 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateGist.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1173 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateMilestoneWithMinimalArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1121 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Milestone.testEditWithMinimalParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1394 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetComments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4157 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCollaborators.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1232 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testEditWithoutParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1108 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Authentication.testOAuthAuthentication.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1101 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTreeWithSha.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    14948 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCompare.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5233 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/GitBlob.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    18368 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Enterprise.testHttp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3372 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue87.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   117727 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testGetGists.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      790 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testGetLabels.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2703 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      382 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/RepositoryKey.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     9119 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequestComment.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2129 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testCreateGist.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1328 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetMembers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11972 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetReposWithArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3763 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Milestone.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      739 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetHooks.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1001 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Authentication.testNoAuthentication.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    36119 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Branch.testCommitCommentsOnLine.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1295 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testCreateIssueComment.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    41736 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchUsers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2671 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateTeamWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1230 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/RateLimiting.testRateLimiting.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4020 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetSubscribers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1660 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testRemoveLabelFromIssue.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   173042 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchReposPagination.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      769 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetContributors.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3557 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetTeams.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4819 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Commit.testGetComments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Label.testEdit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1398 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testLegacySearchIssues.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5834 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/GitTree.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   169972 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetFiles.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1338 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Logging.testLoggingWithOAuthAuthentication.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1598 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testGetLabels.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      386 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Download.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2523 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testMergeWithMessage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5842 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1220 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testAttributes.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      359 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Gist.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    57977 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      640 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Team.testEditWithoutArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    41357 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchReposExplicitPagination.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    52738 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testSliceIndexingInFirstPage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      813 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetAuthorizations.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1226 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Milestone.testEditWithAllParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7653 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3471 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testEditWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6437 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Team.testRepos.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4112 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testDeleteAndSetLabels.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1229 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Logging.testLoggingWithBaseUrl.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1150 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2330 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateRepositoryWithAutoInit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    51406 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetContents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1304 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue54.testConversion.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      983 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetGitRefWithIssue102Reverted.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7735 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreatePullFromIssue.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1487 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateKey.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4987 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetCommits.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1559 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue87.testCreateIssueWithEscapedPercentInTitle.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    22660 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetGitTreeWithRecursive.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5911 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateIssueWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1350 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetMilestones.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2034 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testCreateGistWithoutDescription.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3709 2012-11-19 19:56:53.000000 PyGithub-1.9.1/github/tests/ReplayData/Gist.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1301 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateMilestone.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1867 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testAddLabelToIssue.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    45967 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Event.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1397 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/UserKey.testEditWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    56350 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testGetThirdPage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      747 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetPublicMembers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4640 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/GistComment.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      358 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Team.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    22973 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetStargazers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5048 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testEditWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3925 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/CommitComment.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      382 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Hook.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4502 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetPulls.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3609 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3501 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Download.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7512 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetFollowing.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      859 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateAuthorizationWithoutArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1343 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateIssue.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5073 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Tag.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2788 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   621062 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testSeveralIterations.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    34297 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetOrganizationEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   621062 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testSliceIndexingUntilEnd.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2741 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetRepos.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      983 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetGitRef.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3555 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/GitRef.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1939 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testEditResetMilestone.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1586 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetForks.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1460 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Logging.testLoggingWithBasicAuthentication.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      712 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateTeam.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1562 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testEditWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4289 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetFollowers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1400 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testGetEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5100 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitCommitWithParents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      764 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Authorization.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    60390 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetIssuesWithArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5245 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testEditWithAllParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      382 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Milestone.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      818 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitBlob.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      676 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Team.testEditWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      990 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/RepositoryKey.testEditWithoutParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4019 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue80.testIgnoreHttpsFromGithubEnterpriseWithPort.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    18368 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Enterprise.testSpecificPort.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4928 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetGists.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1825 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateRepositoryWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      884 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/GitRef.testEdit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4755 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetComments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1218 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetIssueComments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      899 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/GitRef.testEditWithForce.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4898 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Team.testMembers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)  1303294 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue33.testClosedIssues.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      725 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetDownloads.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3888 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/Authentication.testSecretKeyAuthentication.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2226 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testMembers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   630715 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue33.testOpenIssues.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2030 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateRepoWithMinimalArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4229 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Authorization.testEdit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1856 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateDownloadWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2743 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetMilestonesWithArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    75894 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1496 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateCommentOnFileLine.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1355 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTagWithAllArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3342 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Gist.testEditWithAllParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3744 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/RepositoryKey.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      848 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Hook.testEditWithMinimalParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3293 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testSetIssueLabels.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    44154 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchRepos.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2744 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetReposWithType.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1248 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTag.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      391 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Exceptions.testBadAuthentication.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3624 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetGitRefs.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    44751 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetPublicEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1256 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testEditWithoutArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1539 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue87.testCreateIssueWithPercentInTitle.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   138453 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetCommits.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2393 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetKeys.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1002 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/GistComment.testEdit.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6572 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateFork.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1368 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateComment.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1398 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testSearchIssues.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1011 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testIssueGetLabels.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     9358 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/CommitStatus.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Exceptions.testInvalidInput.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1535 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue87.testCreateIssueWithPercentInBody.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      912 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateHookWithMinimalParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1536 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetRepo.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4970 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testEditWithoutArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1128 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue.testCreateComment.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    86542 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetIssuesEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2019 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateGistWithoutDescription.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2460 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetArchiveLink.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      380 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Label.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    18366 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetRepos.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1500 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateStatusWithAllParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    52738 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testGetFirstPage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      947 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue50.testCreateLabel.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    48812 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testStarring.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    17224 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testGetHooks.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    58233 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchUsersPagination.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2703 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue33.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2285 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetBranch.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   160299 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testInterruptedIteration.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1911 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Gist.testEditWithoutParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      686 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetOrgs.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      408 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/GitRef.testDelete.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1744 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateDownloadWithMinimalArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3972 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Branch.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10450 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetPullsWithArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    44947 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      949 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateHookWithAllParameters.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   178014 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequestFile.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6950 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateFork.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1006 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitRef.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8387 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testMergeWithCommitMessage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    80111 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetPublicReceivedEvents.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      385 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Hook.testTest.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    52738 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testIntIndexingInFirstPage.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2300 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetStarredGists.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      676 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Markdown.testRenderMarkdown.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      478 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Exceptions.testUnknownUser.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3100 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Organization.testPublicMembers.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1459 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testMerge.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    44098 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testSubscriptions.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4157 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/GitCommit.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1866 2012-11-19 20:40:49.000000 PyGithub-1.9.1/github/tests/ReplayData/Authentication.testUserAgent.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1221 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetIssueComment.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2507 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testEmails.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13052 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetRepos.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    18369 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Enterprise.testHttps.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      877 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateLabel.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10891 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetCommitsWithArguments.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1722 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Team.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1217 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Logging.testLoggingWithoutAuthentication.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3105 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Issue54.setUp.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2280 2012-11-03 09:30:30.000000 PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchUserByEmail.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1795 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/GitRef.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2761 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/RepositoryKey.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2787 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Hook.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2071 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/CommitComment.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7394 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Framework.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1342 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Tag.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4473 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/PaginatedList.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1189 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7545 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Logging_.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2296 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/PullRequestFile.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1244 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Issue33.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2355 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Download.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1594 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Label.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1870 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/CommitStatus.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2930 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Team.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6529 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Organization.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6381 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Gist.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2673 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Milestone.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    30558 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Repository.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    12156 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Github_.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1517 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Markdown.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1040 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/RateLimiting.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6642 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/PullRequest.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1561 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/IssueEvent.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5249 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/Issue.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1810 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/GistComment.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2749 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/tests/UserKey.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1986 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/HookResponse.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10745 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Gist.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7072 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Milestone.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    45033 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Repository.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1923 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GitObject.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2065 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/IssuePullRequest.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1922 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Permissions.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6718 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Requester.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/PullRequestMergeStatus.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    17494 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/PullRequest.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4464 2012-11-20 18:36:28.000000 PyGithub-1.9.1/github/ReadMe.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2500 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/HookDescription.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3901 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/IssueEvent.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13442 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Issue.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3937 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/GistComment.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3625 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/UserKey.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6036 2012-11-20 18:30:53.000000 PyGithub-1.9.1/github/Legacy.py
```

### Comparing `PyGithub-1.9.0/PKG-INFO` & `PyGithub-1.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyGithub
-Version: 1.9.0
+Version: 1.9.1
 Summary: Use the full Github API v3
 Home-page: http://vincent-jacques.net/PyGithub
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: UNKNOWN
 Description: Tutorial
         ========
```

### Comparing `PyGithub-1.9.0/setup.py` & `PyGithub-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if ok:
             exit( 0 )
         else:
             exit( 1 )
 
 setup(
     name = "PyGithub",
-    version = "1.9.0",
+    version = "1.9.1",
     description = "Use the full Github API v3",
     author = "Vincent Jacques",
     author_email = "vincent@vincent-jacques.net",
     url = "http://vincent-jacques.net/PyGithub",
     long_description = textwrap.dedent( """\
         Tutorial
         ========
```

### Comparing `PyGithub-1.9.0/github/AuthorizationApplication.py` & `PyGithub-1.9.1/github/AuthorizationApplication.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/GithubObject.py` & `PyGithub-1.9.1/github/GithubObject.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Branch.py` & `PyGithub-1.9.1/github/Branch.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/GitTree.py` & `PyGithub-1.9.1/github/GitTree.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/InputFileContent.py` & `PyGithub-1.9.1/github/InputFileContent.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/GistHistoryState.py` & `PyGithub-1.9.1/github/GistHistoryState.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Event.py` & `PyGithub-1.9.1/github/Event.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/AuthenticatedUser.py` & `PyGithub-1.9.1/github/AuthenticatedUser.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,15 +327,15 @@
             "/user",
             None,
             post_parameters
         )
         self._useAttributes(data)
 
     def get_authorization(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             "/authorizations/" + str(id),
             None,
             None
         )
         return Authorization.Authorization(self._requester, data, completed=True)
@@ -394,15 +394,15 @@
             Issue.Issue,
             self._requester,
             "/issues",
             None
         )
 
     def get_key(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             "/user/keys/" + str(id),
             None,
             None
         )
         return UserKey.UserKey(self._requester, data, completed=True)
@@ -612,72 +612,72 @@
         if "bio" in attributes:  # pragma no branch
             assert attributes["bio"] is None or isinstance(attributes["bio"], (str, unicode)), attributes["bio"]
             self._bio = attributes["bio"]
         if "blog" in attributes:  # pragma no branch
             assert attributes["blog"] is None or isinstance(attributes["blog"], (str, unicode)), attributes["blog"]
             self._blog = attributes["blog"]
         if "collaborators" in attributes:  # pragma no branch
-            assert attributes["collaborators"] is None or isinstance(attributes["collaborators"], int), attributes["collaborators"]
+            assert attributes["collaborators"] is None or isinstance(attributes["collaborators"], (int, long)), attributes["collaborators"]
             self._collaborators = attributes["collaborators"]
         if "company" in attributes:  # pragma no branch
             assert attributes["company"] is None or isinstance(attributes["company"], (str, unicode)), attributes["company"]
             self._company = attributes["company"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "disk_usage" in attributes:  # pragma no branch
-            assert attributes["disk_usage"] is None or isinstance(attributes["disk_usage"], int), attributes["disk_usage"]
+            assert attributes["disk_usage"] is None or isinstance(attributes["disk_usage"], (int, long)), attributes["disk_usage"]
             self._disk_usage = attributes["disk_usage"]
         if "email" in attributes:  # pragma no branch
             assert attributes["email"] is None or isinstance(attributes["email"], (str, unicode)), attributes["email"]
             self._email = attributes["email"]
         if "followers" in attributes:  # pragma no branch
-            assert attributes["followers"] is None or isinstance(attributes["followers"], int), attributes["followers"]
+            assert attributes["followers"] is None or isinstance(attributes["followers"], (int, long)), attributes["followers"]
             self._followers = attributes["followers"]
         if "following" in attributes:  # pragma no branch
-            assert attributes["following"] is None or isinstance(attributes["following"], int), attributes["following"]
+            assert attributes["following"] is None or isinstance(attributes["following"], (int, long)), attributes["following"]
             self._following = attributes["following"]
         if "gravatar_id" in attributes:  # pragma no branch
             assert attributes["gravatar_id"] is None or isinstance(attributes["gravatar_id"], (str, unicode)), attributes["gravatar_id"]
             self._gravatar_id = attributes["gravatar_id"]
         if "hireable" in attributes:  # pragma no branch
             assert attributes["hireable"] is None or isinstance(attributes["hireable"], bool), attributes["hireable"]
             self._hireable = attributes["hireable"]
         if "html_url" in attributes:  # pragma no branch
             assert attributes["html_url"] is None or isinstance(attributes["html_url"], (str, unicode)), attributes["html_url"]
             self._html_url = attributes["html_url"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "location" in attributes:  # pragma no branch
             assert attributes["location"] is None or isinstance(attributes["location"], (str, unicode)), attributes["location"]
             self._location = attributes["location"]
         if "login" in attributes:  # pragma no branch
             assert attributes["login"] is None or isinstance(attributes["login"], (str, unicode)), attributes["login"]
             self._login = attributes["login"]
         if "name" in attributes:  # pragma no branch
             assert attributes["name"] is None or isinstance(attributes["name"], (str, unicode)), attributes["name"]
             self._name = attributes["name"]
         if "owned_private_repos" in attributes:  # pragma no branch
-            assert attributes["owned_private_repos"] is None or isinstance(attributes["owned_private_repos"], int), attributes["owned_private_repos"]
+            assert attributes["owned_private_repos"] is None or isinstance(attributes["owned_private_repos"], (int, long)), attributes["owned_private_repos"]
             self._owned_private_repos = attributes["owned_private_repos"]
         if "plan" in attributes:  # pragma no branch
             assert attributes["plan"] is None or isinstance(attributes["plan"], dict), attributes["plan"]
             self._plan = None if attributes["plan"] is None else Plan.Plan(self._requester, attributes["plan"], completed=False)
         if "private_gists" in attributes:  # pragma no branch
-            assert attributes["private_gists"] is None or isinstance(attributes["private_gists"], int), attributes["private_gists"]
+            assert attributes["private_gists"] is None or isinstance(attributes["private_gists"], (int, long)), attributes["private_gists"]
             self._private_gists = attributes["private_gists"]
         if "public_gists" in attributes:  # pragma no branch
-            assert attributes["public_gists"] is None or isinstance(attributes["public_gists"], int), attributes["public_gists"]
+            assert attributes["public_gists"] is None or isinstance(attributes["public_gists"], (int, long)), attributes["public_gists"]
             self._public_gists = attributes["public_gists"]
         if "public_repos" in attributes:  # pragma no branch
-            assert attributes["public_repos"] is None or isinstance(attributes["public_repos"], int), attributes["public_repos"]
+            assert attributes["public_repos"] is None or isinstance(attributes["public_repos"], (int, long)), attributes["public_repos"]
             self._public_repos = attributes["public_repos"]
         if "total_private_repos" in attributes:  # pragma no branch
-            assert attributes["total_private_repos"] is None or isinstance(attributes["total_private_repos"], int), attributes["total_private_repos"]
+            assert attributes["total_private_repos"] is None or isinstance(attributes["total_private_repos"], (int, long)), attributes["total_private_repos"]
             self._total_private_repos = attributes["total_private_repos"]
         if "type" in attributes:  # pragma no branch
             assert attributes["type"] is None or isinstance(attributes["type"], (str, unicode)), attributes["type"]
             self._type = attributes["type"]
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/GitBlob.py` & `PyGithub-1.9.1/github/GitBlob.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,12 +56,12 @@
         if "encoding" in attributes:  # pragma no branch
             assert attributes["encoding"] is None or isinstance(attributes["encoding"], (str, unicode)), attributes["encoding"]
             self._encoding = attributes["encoding"]
         if "sha" in attributes:  # pragma no branch
             assert attributes["sha"] is None or isinstance(attributes["sha"], (str, unicode)), attributes["sha"]
             self._sha = attributes["sha"]
         if "size" in attributes:  # pragma no branch
-            assert attributes["size"] is None or isinstance(attributes["size"], int), attributes["size"]
+            assert attributes["size"] is None or isinstance(attributes["size"], (int, long)), attributes["size"]
             self._size = attributes["size"]
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/IssueComment.py` & `PyGithub-1.9.1/github/IssueComment.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         if "body" in attributes:  # pragma no branch
             assert attributes["body"] is None or isinstance(attributes["body"], (str, unicode)), attributes["body"]
             self._body = attributes["body"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "updated_at" in attributes:  # pragma no branch
             assert attributes["updated_at"] is None or isinstance(attributes["updated_at"], (str, unicode)), attributes["updated_at"]
             self._updated_at = self._parseDatetime(attributes["updated_at"])
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/Plan.py` & `PyGithub-1.9.1/github/Plan.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,18 +37,18 @@
         self._collaborators = GithubObject.NotSet
         self._name = GithubObject.NotSet
         self._private_repos = GithubObject.NotSet
         self._space = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "collaborators" in attributes:  # pragma no branch
-            assert attributes["collaborators"] is None or isinstance(attributes["collaborators"], int), attributes["collaborators"]
+            assert attributes["collaborators"] is None or isinstance(attributes["collaborators"], (int, long)), attributes["collaborators"]
             self._collaborators = attributes["collaborators"]
         if "name" in attributes:  # pragma no branch
             assert attributes["name"] is None or isinstance(attributes["name"], (str, unicode)), attributes["name"]
             self._name = attributes["name"]
         if "private_repos" in attributes:  # pragma no branch
-            assert attributes["private_repos"] is None or isinstance(attributes["private_repos"], int), attributes["private_repos"]
+            assert attributes["private_repos"] is None or isinstance(attributes["private_repos"], (int, long)), attributes["private_repos"]
             self._private_repos = attributes["private_repos"]
         if "space" in attributes:  # pragma no branch
-            assert attributes["space"] is None or isinstance(attributes["space"], int), attributes["space"]
+            assert attributes["space"] is None or isinstance(attributes["space"], (int, long)), attributes["space"]
             self._space = attributes["space"]
```

### Comparing `PyGithub-1.9.0/github/GistFile.py` & `PyGithub-1.9.1/github/GistFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,9 +54,9 @@
         if "language" in attributes:  # pragma no branch
             assert attributes["language"] is None or isinstance(attributes["language"], (str, unicode)), attributes["language"]
             self._language = attributes["language"]
         if "raw_url" in attributes:  # pragma no branch
             assert attributes["raw_url"] is None or isinstance(attributes["raw_url"], (str, unicode)), attributes["raw_url"]
             self._raw_url = attributes["raw_url"]
         if "size" in attributes:  # pragma no branch
-            assert attributes["size"] is None or isinstance(attributes["size"], int), attributes["size"]
+            assert attributes["size"] is None or isinstance(attributes["size"], (int, long)), attributes["size"]
             self._size = attributes["size"]
```

### Comparing `PyGithub-1.9.0/github/GitTag.py` & `PyGithub-1.9.1/github/GitTag.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Authorization.py` & `PyGithub-1.9.1/github/Authorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         if "app" in attributes:  # pragma no branch
             assert attributes["app"] is None or isinstance(attributes["app"], dict), attributes["app"]
             self._app = None if attributes["app"] is None else AuthorizationApplication.AuthorizationApplication(self._requester, attributes["app"], completed=False)
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "note" in attributes:  # pragma no branch
             assert attributes["note"] is None or isinstance(attributes["note"], (str, unicode)), attributes["note"]
             self._note = attributes["note"]
         if "note_url" in attributes:  # pragma no branch
             assert attributes["note_url"] is None or isinstance(attributes["note_url"], (str, unicode)), attributes["note_url"]
             self._note_url = attributes["note_url"]
```

### Comparing `PyGithub-1.9.0/github/NamedUser.py` & `PyGithub-1.9.1/github/NamedUser.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,75 +323,75 @@
         if "bio" in attributes:  # pragma no branch
             assert attributes["bio"] is None or isinstance(attributes["bio"], (str, unicode)), attributes["bio"]
             self._bio = attributes["bio"]
         if "blog" in attributes:  # pragma no branch
             assert attributes["blog"] is None or isinstance(attributes["blog"], (str, unicode)), attributes["blog"]
             self._blog = attributes["blog"]
         if "collaborators" in attributes:  # pragma no branch
-            assert attributes["collaborators"] is None or isinstance(attributes["collaborators"], int), attributes["collaborators"]
+            assert attributes["collaborators"] is None or isinstance(attributes["collaborators"], (int, long)), attributes["collaborators"]
             self._collaborators = attributes["collaborators"]
         if "company" in attributes:  # pragma no branch
             assert attributes["company"] is None or isinstance(attributes["company"], (str, unicode)), attributes["company"]
             self._company = attributes["company"]
         if "contributions" in attributes:  # pragma no branch
-            assert attributes["contributions"] is None or isinstance(attributes["contributions"], int), attributes["contributions"]
+            assert attributes["contributions"] is None or isinstance(attributes["contributions"], (int, long)), attributes["contributions"]
             self._contributions = attributes["contributions"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "disk_usage" in attributes:  # pragma no branch
-            assert attributes["disk_usage"] is None or isinstance(attributes["disk_usage"], int), attributes["disk_usage"]
+            assert attributes["disk_usage"] is None or isinstance(attributes["disk_usage"], (int, long)), attributes["disk_usage"]
             self._disk_usage = attributes["disk_usage"]
         if "email" in attributes:  # pragma no branch
             assert attributes["email"] is None or isinstance(attributes["email"], (str, unicode)), attributes["email"]
             self._email = attributes["email"]
         if "followers" in attributes:  # pragma no branch
-            assert attributes["followers"] is None or isinstance(attributes["followers"], int), attributes["followers"]
+            assert attributes["followers"] is None or isinstance(attributes["followers"], (int, long)), attributes["followers"]
             self._followers = attributes["followers"]
         if "following" in attributes:  # pragma no branch
-            assert attributes["following"] is None or isinstance(attributes["following"], int), attributes["following"]
+            assert attributes["following"] is None or isinstance(attributes["following"], (int, long)), attributes["following"]
             self._following = attributes["following"]
         if "gravatar_id" in attributes:  # pragma no branch
             assert attributes["gravatar_id"] is None or isinstance(attributes["gravatar_id"], (str, unicode)), attributes["gravatar_id"]
             self._gravatar_id = attributes["gravatar_id"]
         if "hireable" in attributes:  # pragma no branch
             assert attributes["hireable"] is None or isinstance(attributes["hireable"], bool), attributes["hireable"]
             self._hireable = attributes["hireable"]
         if "html_url" in attributes:  # pragma no branch
             assert attributes["html_url"] is None or isinstance(attributes["html_url"], (str, unicode)), attributes["html_url"]
             self._html_url = attributes["html_url"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "location" in attributes:  # pragma no branch
             assert attributes["location"] is None or isinstance(attributes["location"], (str, unicode)), attributes["location"]
             self._location = attributes["location"]
         if "login" in attributes:  # pragma no branch
             assert attributes["login"] is None or isinstance(attributes["login"], (str, unicode)), attributes["login"]
             self._login = attributes["login"]
         if "name" in attributes:  # pragma no branch
             assert attributes["name"] is None or isinstance(attributes["name"], (str, unicode)), attributes["name"]
             self._name = attributes["name"]
         if "owned_private_repos" in attributes:  # pragma no branch
-            assert attributes["owned_private_repos"] is None or isinstance(attributes["owned_private_repos"], int), attributes["owned_private_repos"]
+            assert attributes["owned_private_repos"] is None or isinstance(attributes["owned_private_repos"], (int, long)), attributes["owned_private_repos"]
             self._owned_private_repos = attributes["owned_private_repos"]
         if "plan" in attributes:  # pragma no branch
             assert attributes["plan"] is None or isinstance(attributes["plan"], dict), attributes["plan"]
             self._plan = None if attributes["plan"] is None else Plan.Plan(self._requester, attributes["plan"], completed=False)
         if "private_gists" in attributes:  # pragma no branch
-            assert attributes["private_gists"] is None or isinstance(attributes["private_gists"], int), attributes["private_gists"]
+            assert attributes["private_gists"] is None or isinstance(attributes["private_gists"], (int, long)), attributes["private_gists"]
             self._private_gists = attributes["private_gists"]
         if "public_gists" in attributes:  # pragma no branch
-            assert attributes["public_gists"] is None or isinstance(attributes["public_gists"], int), attributes["public_gists"]
+            assert attributes["public_gists"] is None or isinstance(attributes["public_gists"], (int, long)), attributes["public_gists"]
             self._public_gists = attributes["public_gists"]
         if "public_repos" in attributes:  # pragma no branch
-            assert attributes["public_repos"] is None or isinstance(attributes["public_repos"], int), attributes["public_repos"]
+            assert attributes["public_repos"] is None or isinstance(attributes["public_repos"], (int, long)), attributes["public_repos"]
             self._public_repos = attributes["public_repos"]
         if "total_private_repos" in attributes:  # pragma no branch
-            assert attributes["total_private_repos"] is None or isinstance(attributes["total_private_repos"], int), attributes["total_private_repos"]
+            assert attributes["total_private_repos"] is None or isinstance(attributes["total_private_repos"], (int, long)), attributes["total_private_repos"]
             self._total_private_repos = attributes["total_private_repos"]
         if "type" in attributes:  # pragma no branch
             assert attributes["type"] is None or isinstance(attributes["type"], (str, unicode)), attributes["type"]
             self._type = attributes["type"]
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/PullRequestComment.py` & `PyGithub-1.9.1/github/PullRequestComment.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,27 +115,27 @@
         if "commit_id" in attributes:  # pragma no branch
             assert attributes["commit_id"] is None or isinstance(attributes["commit_id"], (str, unicode)), attributes["commit_id"]
             self._commit_id = attributes["commit_id"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "original_commit_id" in attributes:  # pragma no branch
             assert attributes["original_commit_id"] is None or isinstance(attributes["original_commit_id"], (str, unicode)), attributes["original_commit_id"]
             self._original_commit_id = attributes["original_commit_id"]
         if "original_position" in attributes:  # pragma no branch
-            assert attributes["original_position"] is None or isinstance(attributes["original_position"], int), attributes["original_position"]
+            assert attributes["original_position"] is None or isinstance(attributes["original_position"], (int, long)), attributes["original_position"]
             self._original_position = attributes["original_position"]
         if "path" in attributes:  # pragma no branch
             assert attributes["path"] is None or isinstance(attributes["path"], (str, unicode)), attributes["path"]
             self._path = attributes["path"]
         if "position" in attributes:  # pragma no branch
-            assert attributes["position"] is None or isinstance(attributes["position"], int), attributes["position"]
+            assert attributes["position"] is None or isinstance(attributes["position"], (int, long)), attributes["position"]
             self._position = attributes["position"]
         if "updated_at" in attributes:  # pragma no branch
             assert attributes["updated_at"] is None or isinstance(attributes["updated_at"], (str, unicode)), attributes["updated_at"]
             self._updated_at = self._parseDatetime(attributes["updated_at"])
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/File.py` & `PyGithub-1.9.1/github/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,24 +62,24 @@
         self._patch = GithubObject.NotSet
         self._raw_url = GithubObject.NotSet
         self._sha = GithubObject.NotSet
         self._status = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "additions" in attributes:  # pragma no branch
-            assert attributes["additions"] is None or isinstance(attributes["additions"], int), attributes["additions"]
+            assert attributes["additions"] is None or isinstance(attributes["additions"], (int, long)), attributes["additions"]
             self._additions = attributes["additions"]
         if "blob_url" in attributes:  # pragma no branch
             assert attributes["blob_url"] is None or isinstance(attributes["blob_url"], (str, unicode)), attributes["blob_url"]
             self._blob_url = attributes["blob_url"]
         if "changes" in attributes:  # pragma no branch
-            assert attributes["changes"] is None or isinstance(attributes["changes"], int), attributes["changes"]
+            assert attributes["changes"] is None or isinstance(attributes["changes"], (int, long)), attributes["changes"]
             self._changes = attributes["changes"]
         if "deletions" in attributes:  # pragma no branch
-            assert attributes["deletions"] is None or isinstance(attributes["deletions"], int), attributes["deletions"]
+            assert attributes["deletions"] is None or isinstance(attributes["deletions"], (int, long)), attributes["deletions"]
             self._deletions = attributes["deletions"]
         if "filename" in attributes:  # pragma no branch
             assert attributes["filename"] is None or isinstance(attributes["filename"], (str, unicode)), attributes["filename"]
             self._filename = attributes["filename"]
         if "patch" in attributes:  # pragma no branch
             assert attributes["patch"] is None or isinstance(attributes["patch"], (str, unicode)), attributes["patch"]
             self._patch = attributes["patch"]
```

### Comparing `PyGithub-1.9.0/github/Commit.py` & `PyGithub-1.9.1/github/Commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,17 @@
     @property
     def url(self):
         self._completeIfNotSet(self._url)
         return self._NoneIfNotSet(self._url)
 
     def create_comment(self, body, line=GithubObject.NotSet, path=GithubObject.NotSet, position=GithubObject.NotSet):
         assert isinstance(body, (str, unicode)), body
-        assert line is GithubObject.NotSet or isinstance(line, int), line
+        assert line is GithubObject.NotSet or isinstance(line, (int, long)), line
         assert path is GithubObject.NotSet or isinstance(path, (str, unicode)), path
-        assert position is GithubObject.NotSet or isinstance(position, int), position
+        assert position is GithubObject.NotSet or isinstance(position, (int, long)), position
         post_parameters = {
             "body": body,
         }
         if line is not GithubObject.NotSet:
             post_parameters["line"] = line
         if path is not GithubObject.NotSet:
             post_parameters["path"] = path
```

### Comparing `PyGithub-1.9.0/github/GitCommit.py` & `PyGithub-1.9.1/github/GitCommit.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/ContentFile.py` & `PyGithub-1.9.1/github/ContentFile.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,12 +67,12 @@
         if "path" in attributes:  # pragma no branch
             assert attributes["path"] is None or isinstance(attributes["path"], (str, unicode)), attributes["path"]
             self._path = attributes["path"]
         if "sha" in attributes:  # pragma no branch
             assert attributes["sha"] is None or isinstance(attributes["sha"], (str, unicode)), attributes["sha"]
             self._sha = attributes["sha"]
         if "size" in attributes:  # pragma no branch
-            assert attributes["size"] is None or isinstance(attributes["size"], int), attributes["size"]
+            assert attributes["size"] is None or isinstance(attributes["size"], (int, long)), attributes["size"]
             self._size = attributes["size"]
         if "type" in attributes:  # pragma no branch
             assert attributes["type"] is None or isinstance(attributes["type"], (str, unicode)), attributes["type"]
             self._type = attributes["type"]
```

### Comparing `PyGithub-1.9.0/github/GitRef.py` & `PyGithub-1.9.1/github/GitRef.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/RepositoryKey.py` & `PyGithub-1.9.1/github/RepositoryKey.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self._key = GithubObject.NotSet
         self._title = GithubObject.NotSet
         self._url = GithubObject.NotSet
         self._verified = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "key" in attributes:  # pragma no branch
             assert attributes["key"] is None or isinstance(attributes["key"], (str, unicode)), attributes["key"]
             self._key = attributes["key"]
         if "title" in attributes:  # pragma no branch
             assert attributes["title"] is None or isinstance(attributes["title"], (str, unicode)), attributes["title"]
             self._title = attributes["title"]
```

### Comparing `PyGithub-1.9.0/github/GitTreeElement.py` & `PyGithub-1.9.1/github/GitTreeElement.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         if "path" in attributes:  # pragma no branch
             assert attributes["path"] is None or isinstance(attributes["path"], (str, unicode)), attributes["path"]
             self._path = attributes["path"]
         if "sha" in attributes:  # pragma no branch
             assert attributes["sha"] is None or isinstance(attributes["sha"], (str, unicode)), attributes["sha"]
             self._sha = attributes["sha"]
         if "size" in attributes:  # pragma no branch
-            assert attributes["size"] is None or isinstance(attributes["size"], int), attributes["size"]
+            assert attributes["size"] is None or isinstance(attributes["size"], (int, long)), attributes["size"]
             self._size = attributes["size"]
         if "type" in attributes:  # pragma no branch
             assert attributes["type"] is None or isinstance(attributes["type"], (str, unicode)), attributes["type"]
             self._type = attributes["type"]
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/PullRequestPart.py` & `PyGithub-1.9.1/github/PullRequestPart.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Hook.py` & `PyGithub-1.9.1/github/Hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "events" in attributes:  # pragma no branch
             assert attributes["events"] is None or all(isinstance(element, (str, unicode)) for element in attributes["events"]), attributes["events"]
             self._events = attributes["events"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "last_response" in attributes:  # pragma no branch
             assert attributes["last_response"] is None or isinstance(attributes["last_response"], dict), attributes["last_response"]
             self._last_response = None if attributes["last_response"] is None else HookResponse.HookResponse(self._requester, attributes["last_response"], completed=False)
         if "name" in attributes:  # pragma no branch
             assert attributes["name"] is None or isinstance(attributes["name"], (str, unicode)), attributes["name"]
             self._name = attributes["name"]
```

### Comparing `PyGithub-1.9.0/github/Github.py` & `PyGithub-1.9.1/github/Github.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/CommitComment.py` & `PyGithub-1.9.1/github/CommitComment.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,24 +118,24 @@
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "html_url" in attributes:  # pragma no branch
             assert attributes["html_url"] is None or isinstance(attributes["html_url"], (str, unicode)), attributes["html_url"]
             self._html_url = attributes["html_url"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "line" in attributes:  # pragma no branch
-            assert attributes["line"] is None or isinstance(attributes["line"], int), attributes["line"]
+            assert attributes["line"] is None or isinstance(attributes["line"], (int, long)), attributes["line"]
             self._line = attributes["line"]
         if "path" in attributes:  # pragma no branch
             assert attributes["path"] is None or isinstance(attributes["path"], (str, unicode)), attributes["path"]
             self._path = attributes["path"]
         if "position" in attributes:  # pragma no branch
-            assert attributes["position"] is None or isinstance(attributes["position"], int), attributes["position"]
+            assert attributes["position"] is None or isinstance(attributes["position"], (int, long)), attributes["position"]
             self._position = attributes["position"]
         if "updated_at" in attributes:  # pragma no branch
             assert attributes["updated_at"] is None or isinstance(attributes["updated_at"], (str, unicode)), attributes["updated_at"]
             self._updated_at = self._parseDatetime(attributes["updated_at"])
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/InputGitTreeElement.py` & `PyGithub-1.9.1/github/InputGitTreeElement.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Tag.py` & `PyGithub-1.9.1/github/Tag.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/InputGitAuthor.py` & `PyGithub-1.9.1/github/InputGitAuthor.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Comparison.py` & `PyGithub-1.9.1/github/Comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,21 +92,21 @@
         self._permalink_url = GithubObject.NotSet
         self._status = GithubObject.NotSet
         self._total_commits = GithubObject.NotSet
         self._url = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "ahead_by" in attributes:  # pragma no branch
-            assert attributes["ahead_by"] is None or isinstance(attributes["ahead_by"], int), attributes["ahead_by"]
+            assert attributes["ahead_by"] is None or isinstance(attributes["ahead_by"], (int, long)), attributes["ahead_by"]
             self._ahead_by = attributes["ahead_by"]
         if "base_commit" in attributes:  # pragma no branch
             assert attributes["base_commit"] is None or isinstance(attributes["base_commit"], dict), attributes["base_commit"]
             self._base_commit = None if attributes["base_commit"] is None else Commit.Commit(self._requester, attributes["base_commit"], completed=False)
         if "behind_by" in attributes:  # pragma no branch
-            assert attributes["behind_by"] is None or isinstance(attributes["behind_by"], int), attributes["behind_by"]
+            assert attributes["behind_by"] is None or isinstance(attributes["behind_by"], (int, long)), attributes["behind_by"]
             self._behind_by = attributes["behind_by"]
         if "commits" in attributes:  # pragma no branch
             assert attributes["commits"] is None or all(isinstance(element, dict) for element in attributes["commits"]), attributes["commits"]
             self._commits = None if attributes["commits"] is None else [
                 Commit.Commit(self._requester, element, completed=False)
                 for element in attributes["commits"]
             ]
@@ -128,12 +128,12 @@
         if "permalink_url" in attributes:  # pragma no branch
             assert attributes["permalink_url"] is None or isinstance(attributes["permalink_url"], (str, unicode)), attributes["permalink_url"]
             self._permalink_url = attributes["permalink_url"]
         if "status" in attributes:  # pragma no branch
             assert attributes["status"] is None or isinstance(attributes["status"], (str, unicode)), attributes["status"]
             self._status = attributes["status"]
         if "total_commits" in attributes:  # pragma no branch
-            assert attributes["total_commits"] is None or isinstance(attributes["total_commits"], int), attributes["total_commits"]
+            assert attributes["total_commits"] is None or isinstance(attributes["total_commits"], (int, long)), attributes["total_commits"]
             self._total_commits = attributes["total_commits"]
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/PaginatedList.py` & `PyGithub-1.9.1/github/PaginatedList.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class PaginatedListBase:
     def __init__(self):
         self.__elements = list()
 
     def __getitem__(self, index):
         assert isinstance(index, (int, slice))
-        if isinstance(index, int):
+        if isinstance(index, (int, long)):
             self.__fetchToIndex(index)
             return self.__elements[index]
         else:
             return self._Slice(self, index)
 
     def __iter__(self):
         for element in self.__elements:
```

### Comparing `PyGithub-1.9.0/github/__init__.py` & `PyGithub-1.9.1/github/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Download.py` & `PyGithub-1.9.1/github/Download.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,24 +163,24 @@
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "description" in attributes:  # pragma no branch
             assert attributes["description"] is None or isinstance(attributes["description"], (str, unicode)), attributes["description"]
             self._description = attributes["description"]
         if "download_count" in attributes:  # pragma no branch
-            assert attributes["download_count"] is None or isinstance(attributes["download_count"], int), attributes["download_count"]
+            assert attributes["download_count"] is None or isinstance(attributes["download_count"], (int, long)), attributes["download_count"]
             self._download_count = attributes["download_count"]
         if "expirationdate" in attributes:  # pragma no branch
             assert attributes["expirationdate"] is None or isinstance(attributes["expirationdate"], (str, unicode)), attributes["expirationdate"]
             self._expirationdate = self._parseDatetime(attributes["expirationdate"])
         if "html_url" in attributes:  # pragma no branch
             assert attributes["html_url"] is None or isinstance(attributes["html_url"], (str, unicode)), attributes["html_url"]
             self._html_url = attributes["html_url"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "mime_type" in attributes:  # pragma no branch
             assert attributes["mime_type"] is None or isinstance(attributes["mime_type"], (str, unicode)), attributes["mime_type"]
             self._mime_type = attributes["mime_type"]
         if "name" in attributes:  # pragma no branch
             assert attributes["name"] is None or isinstance(attributes["name"], (str, unicode)), attributes["name"]
             self._name = attributes["name"]
@@ -199,12 +199,12 @@
         if "s3_url" in attributes:  # pragma no branch
             assert attributes["s3_url"] is None or isinstance(attributes["s3_url"], (str, unicode)), attributes["s3_url"]
             self._s3_url = attributes["s3_url"]
         if "signature" in attributes:  # pragma no branch
             assert attributes["signature"] is None or isinstance(attributes["signature"], (str, unicode)), attributes["signature"]
             self._signature = attributes["signature"]
         if "size" in attributes:  # pragma no branch
-            assert attributes["size"] is None or isinstance(attributes["size"], int), attributes["size"]
+            assert attributes["size"] is None or isinstance(attributes["size"], (int, long)), attributes["size"]
             self._size = attributes["size"]
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/CommitStats.py` & `PyGithub-1.9.1/github/CommitStats.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def _initAttributes(self):
         self._additions = GithubObject.NotSet
         self._deletions = GithubObject.NotSet
         self._total = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "additions" in attributes:  # pragma no branch
-            assert attributes["additions"] is None or isinstance(attributes["additions"], int), attributes["additions"]
+            assert attributes["additions"] is None or isinstance(attributes["additions"], (int, long)), attributes["additions"]
             self._additions = attributes["additions"]
         if "deletions" in attributes:  # pragma no branch
-            assert attributes["deletions"] is None or isinstance(attributes["deletions"], int), attributes["deletions"]
+            assert attributes["deletions"] is None or isinstance(attributes["deletions"], (int, long)), attributes["deletions"]
             self._deletions = attributes["deletions"]
         if "total" in attributes:  # pragma no branch
-            assert attributes["total"] is None or isinstance(attributes["total"], int), attributes["total"]
+            assert attributes["total"] is None or isinstance(attributes["total"], (int, long)), attributes["total"]
             self._total = attributes["total"]
```

### Comparing `PyGithub-1.9.0/github/Label.py` & `PyGithub-1.9.1/github/Label.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/GithubException.py` & `PyGithub-1.9.1/github/GithubException.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/GitAuthor.py` & `PyGithub-1.9.1/github/GitAuthor.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/CommitStatus.py` & `PyGithub-1.9.1/github/CommitStatus.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         if "creator" in attributes:  # pragma no branch
             assert attributes["creator"] is None or isinstance(attributes["creator"], dict), attributes["creator"]
             self._creator = None if attributes["creator"] is None else NamedUser.NamedUser(self._requester, attributes["creator"], completed=False)
         if "description" in attributes:  # pragma no branch
             assert attributes["description"] is None or isinstance(attributes["description"], (str, unicode)), attributes["description"]
             self._description = attributes["description"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "state" in attributes:  # pragma no branch
             assert attributes["state"] is None or isinstance(attributes["state"], (str, unicode)), attributes["state"]
             self._state = attributes["state"]
         if "target_url" in attributes:  # pragma no branch
             assert attributes["target_url"] is None or isinstance(attributes["target_url"], (str, unicode)), attributes["target_url"]
             self._target_url = attributes["target_url"]
```

### Comparing `PyGithub-1.9.0/github/Team.py` & `PyGithub-1.9.1/github/Team.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,24 +157,24 @@
         self._name = GithubObject.NotSet
         self._permission = GithubObject.NotSet
         self._repos_count = GithubObject.NotSet
         self._url = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "members_count" in attributes:  # pragma no branch
-            assert attributes["members_count"] is None or isinstance(attributes["members_count"], int), attributes["members_count"]
+            assert attributes["members_count"] is None or isinstance(attributes["members_count"], (int, long)), attributes["members_count"]
             self._members_count = attributes["members_count"]
         if "name" in attributes:  # pragma no branch
             assert attributes["name"] is None or isinstance(attributes["name"], (str, unicode)), attributes["name"]
             self._name = attributes["name"]
         if "permission" in attributes:  # pragma no branch
             assert attributes["permission"] is None or isinstance(attributes["permission"], (str, unicode)), attributes["permission"]
             self._permission = attributes["permission"]
         if "repos_count" in attributes:  # pragma no branch
-            assert attributes["repos_count"] is None or isinstance(attributes["repos_count"], int), attributes["repos_count"]
+            assert attributes["repos_count"] is None or isinstance(attributes["repos_count"], (int, long)), attributes["repos_count"]
             self._repos_count = attributes["repos_count"]
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/Organization.py` & `PyGithub-1.9.1/github/Organization.py`

 * *Files 3% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             Repository.Repository,
             self._requester,
             self.url + "/repos",
             url_parameters
         )
 
     def get_team(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             "/teams/" + str(id),
             None,
             None
         )
         return Team.Team(self._requester, data, completed=True)
@@ -388,69 +388,69 @@
         if "billing_email" in attributes:  # pragma no branch
             assert attributes["billing_email"] is None or isinstance(attributes["billing_email"], (str, unicode)), attributes["billing_email"]
             self._billing_email = attributes["billing_email"]
         if "blog" in attributes:  # pragma no branch
             assert attributes["blog"] is None or isinstance(attributes["blog"], (str, unicode)), attributes["blog"]
             self._blog = attributes["blog"]
         if "collaborators" in attributes:  # pragma no branch
-            assert attributes["collaborators"] is None or isinstance(attributes["collaborators"], int), attributes["collaborators"]
+            assert attributes["collaborators"] is None or isinstance(attributes["collaborators"], (int, long)), attributes["collaborators"]
             self._collaborators = attributes["collaborators"]
         if "company" in attributes:  # pragma no branch
             assert attributes["company"] is None or isinstance(attributes["company"], (str, unicode)), attributes["company"]
             self._company = attributes["company"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "disk_usage" in attributes:  # pragma no branch
-            assert attributes["disk_usage"] is None or isinstance(attributes["disk_usage"], int), attributes["disk_usage"]
+            assert attributes["disk_usage"] is None or isinstance(attributes["disk_usage"], (int, long)), attributes["disk_usage"]
             self._disk_usage = attributes["disk_usage"]
         if "email" in attributes:  # pragma no branch
             assert attributes["email"] is None or isinstance(attributes["email"], (str, unicode)), attributes["email"]
             self._email = attributes["email"]
         if "followers" in attributes:  # pragma no branch
-            assert attributes["followers"] is None or isinstance(attributes["followers"], int), attributes["followers"]
+            assert attributes["followers"] is None or isinstance(attributes["followers"], (int, long)), attributes["followers"]
             self._followers = attributes["followers"]
         if "following" in attributes:  # pragma no branch
-            assert attributes["following"] is None or isinstance(attributes["following"], int), attributes["following"]
+            assert attributes["following"] is None or isinstance(attributes["following"], (int, long)), attributes["following"]
             self._following = attributes["following"]
         if "gravatar_id" in attributes:  # pragma no branch
             assert attributes["gravatar_id"] is None or isinstance(attributes["gravatar_id"], (str, unicode)), attributes["gravatar_id"]
             self._gravatar_id = attributes["gravatar_id"]
         if "html_url" in attributes:  # pragma no branch
             assert attributes["html_url"] is None or isinstance(attributes["html_url"], (str, unicode)), attributes["html_url"]
             self._html_url = attributes["html_url"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "location" in attributes:  # pragma no branch
             assert attributes["location"] is None or isinstance(attributes["location"], (str, unicode)), attributes["location"]
             self._location = attributes["location"]
         if "login" in attributes:  # pragma no branch
             assert attributes["login"] is None or isinstance(attributes["login"], (str, unicode)), attributes["login"]
             self._login = attributes["login"]
         if "name" in attributes:  # pragma no branch
             assert attributes["name"] is None or isinstance(attributes["name"], (str, unicode)), attributes["name"]
             self._name = attributes["name"]
         if "owned_private_repos" in attributes:  # pragma no branch
-            assert attributes["owned_private_repos"] is None or isinstance(attributes["owned_private_repos"], int), attributes["owned_private_repos"]
+            assert attributes["owned_private_repos"] is None or isinstance(attributes["owned_private_repos"], (int, long)), attributes["owned_private_repos"]
             self._owned_private_repos = attributes["owned_private_repos"]
         if "plan" in attributes:  # pragma no branch
             assert attributes["plan"] is None or isinstance(attributes["plan"], dict), attributes["plan"]
             self._plan = None if attributes["plan"] is None else Plan.Plan(self._requester, attributes["plan"], completed=False)
         if "private_gists" in attributes:  # pragma no branch
-            assert attributes["private_gists"] is None or isinstance(attributes["private_gists"], int), attributes["private_gists"]
+            assert attributes["private_gists"] is None or isinstance(attributes["private_gists"], (int, long)), attributes["private_gists"]
             self._private_gists = attributes["private_gists"]
         if "public_gists" in attributes:  # pragma no branch
-            assert attributes["public_gists"] is None or isinstance(attributes["public_gists"], int), attributes["public_gists"]
+            assert attributes["public_gists"] is None or isinstance(attributes["public_gists"], (int, long)), attributes["public_gists"]
             self._public_gists = attributes["public_gists"]
         if "public_repos" in attributes:  # pragma no branch
-            assert attributes["public_repos"] is None or isinstance(attributes["public_repos"], int), attributes["public_repos"]
+            assert attributes["public_repos"] is None or isinstance(attributes["public_repos"], (int, long)), attributes["public_repos"]
             self._public_repos = attributes["public_repos"]
         if "total_private_repos" in attributes:  # pragma no branch
-            assert attributes["total_private_repos"] is None or isinstance(attributes["total_private_repos"], int), attributes["total_private_repos"]
+            assert attributes["total_private_repos"] is None or isinstance(attributes["total_private_repos"], (int, long)), attributes["total_private_repos"]
             self._total_private_repos = attributes["total_private_repos"]
         if "type" in attributes:  # pragma no branch
             assert attributes["type"] is None or isinstance(attributes["type"], (str, unicode)), attributes["type"]
             self._type = attributes["type"]
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/tests/IntegrationTest.py` & `PyGithub-1.9.1/github/tests/IntegrationTest.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Branch.py` & `PyGithub-1.9.1/github/tests/Branch.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/GitTree.py` & `PyGithub-1.9.1/github/tests/GitTree.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Exceptions.py` & `PyGithub-1.9.1/github/tests/Exceptions.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Issue50.py` & `PyGithub-1.9.1/github/tests/Issue50.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Event.py` & `PyGithub-1.9.1/github/tests/Event.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/AuthenticatedUser.py` & `PyGithub-1.9.1/github/tests/AuthenticatedUser.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/GitBlob.py` & `PyGithub-1.9.1/github/tests/GitBlob.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/IssueComment.py` & `PyGithub-1.9.1/github/tests/IssueComment.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Issue54.py` & `PyGithub-1.9.1/github/tests/Issue54.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/GitTag.py` & `PyGithub-1.9.1/github/tests/GitTag.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Issue80.py` & `PyGithub-1.9.1/github/tests/Issue80.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Authentication.py` & `PyGithub-1.9.1/github/tests/Authentication.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Issue87.py` & `PyGithub-1.9.1/github/tests/Issue87.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Authorization.py` & `PyGithub-1.9.1/github/tests/Authorization.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/NamedUser.py` & `PyGithub-1.9.1/github/tests/NamedUser.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/PullRequestComment.py` & `PyGithub-1.9.1/github/tests/PullRequestComment.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/AllTests.py` & `PyGithub-1.9.1/github/tests/AllTests.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Commit.py` & `PyGithub-1.9.1/github/tests/Commit.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/__main__.py` & `PyGithub-1.9.1/github/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/GitCommit.py` & `PyGithub-1.9.1/github/tests/GitCommit.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Enterprise.py` & `PyGithub-1.9.1/github/tests/Enterprise.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ContentFile.py` & `PyGithub-1.9.1/github/tests/ContentFile.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testGetLabel.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testGetLabel.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetSubscriptions.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetSubscriptions.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateRepositoryWithAutoInit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateRepositoryWithAutoInit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testGetComments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testGetComments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/IssueEvent.testAttributes.txt` & `PyGithub-1.9.1/github/tests/ReplayData/IssueEvent.testAttributes.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue87.testCreateIssueWithEscapedPercentInBody.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue87.testCreateIssueWithEscapedPercentInBody.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/UserKey.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/UserKey.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetIssues.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetIssues.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/RepositoryKey.testEdit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/RepositoryKey.testEdit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testFollowing.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testFollowing.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testSearchRepos.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testSearchRepos.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testEditWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testEditWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetTeams.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetTeams.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testAttributesOfOtherUser.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testAttributesOfOtherUser.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Markdown.testRenderGithubFlavoredMarkdown.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Markdown.testRenderGithubFlavoredMarkdown.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetIssues.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetIssues.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Gist.testGetComments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Gist.testGetComments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/CommitComment.testEdit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/CommitComment.testEdit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue80.testIgnoreHttpsFromGithubEnterprise.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue80.testIgnoreHttpsFromGithubEnterprise.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testWatching.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testWatching.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Enterprise.testLongUrl.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Enterprise.testLongUrl.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testAssignees.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testAssignees.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testIntIndexingAfterIteration.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testIntIndexingAfterIteration.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testIteration.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testIteration.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testCreateComment.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testCreateComment.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testInterruptedIterationInSlice.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testInterruptedIterationInSlice.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateRepository.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateRepository.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/IssueComment.testEdit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/IssueComment.testEdit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetWatchers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetWatchers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testMergeWithoutMessage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testMergeWithoutMessage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitCommit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitCommit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Milestone.testGetLabels.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Milestone.testGetLabels.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/UserKey.testEditWithoutArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/UserKey.testEditWithoutArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTreeWithBaseTree.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTreeWithBaseTree.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateAuthorizationWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateAuthorizationWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testSliceIndexingUntilFourthPage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testSliceIndexingUntilFourthPage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Gist.testStarring.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Gist.testStarring.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testMergeWithConflict.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testMergeWithConflict.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Markdown.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Markdown.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testIntIndexingInThirdPage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testIntIndexingInThirdPage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Authentication.testBasicAuthentication.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Authentication.testBasicAuthentication.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Hook.testEditWithAllParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Hook.testEditWithAllParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Gist.testCreateComment.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Gist.testCreateComment.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testEditResetAssignee.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testEditResetAssignee.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetKeys.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetKeys.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequestComment.testEdit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequestComment.testEdit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/ContentFile.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/ContentFile.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetWatched.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetWatched.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetReceivedEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetReceivedEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testMergeWithNothingToDo.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testMergeWithNothingToDo.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testSearchUserByEmail.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testSearchUserByEmail.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testAddAndRemoveLabels.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testAddAndRemoveLabels.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateCommentOnFilePosition.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateCommentOnFilePosition.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testCreateIssueWithLabel.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testCreateIssueWithLabel.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateRepoWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateRepoWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchReposWithLanguage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchReposWithLanguage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testSearchUsers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testSearchUsers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateKey.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateKey.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testEditWithDefaultBranch.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testEditWithDefaultBranch.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitCommitWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitCommitWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetLabel.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetLabel.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchUsersExplicitPagination.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchUsersExplicitPagination.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testEditWithoutArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testEditWithoutArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetStarred.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetStarred.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/IssueEvent.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/IssueEvent.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetLabels.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetLabels.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetReposWithType.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetReposWithType.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Label.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Label.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/IssueComment.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/IssueComment.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GitTag.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GitTag.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Exceptions.testUnknownObject.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Exceptions.testUnknownObject.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Commit.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Commit.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateStatusWithoutOptionalParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateStatusWithoutOptionalParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetOrgs.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetOrgs.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetNetworkEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetNetworkEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Gist.testFork.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Gist.testFork.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetIssuesWithWildcards.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetIssuesWithWildcards.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTree.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTree.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testGetIssuesWithLabel.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testGetIssuesWithLabel.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetGists.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetGists.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Hook.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Hook.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreatePull.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreatePull.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testEditWithoutArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testEditWithoutArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateGist.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateGist.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateMilestoneWithMinimalArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateMilestoneWithMinimalArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Milestone.testEditWithMinimalParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Milestone.testEditWithMinimalParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetComments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetComments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCollaborators.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCollaborators.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testEditWithoutParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testEditWithoutParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Authentication.testOAuthAuthentication.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Authentication.testOAuthAuthentication.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTreeWithSha.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTreeWithSha.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCompare.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCompare.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GitBlob.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GitBlob.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Enterprise.testHttp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Enterprise.testHttp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue87.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue87.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testGetGists.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testGetGists.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testGetLabels.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testGetLabels.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequestComment.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequestComment.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testCreateGist.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testCreateGist.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetMembers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetMembers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetReposWithArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetReposWithArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Milestone.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Milestone.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetHooks.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetHooks.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Authentication.testNoAuthentication.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Authentication.testNoAuthentication.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Branch.testCommitCommentsOnLine.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Branch.testCommitCommentsOnLine.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testCreateIssueComment.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testCreateIssueComment.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchUsers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchUsers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateTeamWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateTeamWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/RateLimiting.testRateLimiting.txt` & `PyGithub-1.9.1/github/tests/ReplayData/RateLimiting.testRateLimiting.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetSubscribers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetSubscribers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testRemoveLabelFromIssue.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testRemoveLabelFromIssue.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchReposPagination.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchReposPagination.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetContributors.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetContributors.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetTeams.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetTeams.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Commit.testGetComments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Commit.testGetComments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Label.testEdit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Label.testEdit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testLegacySearchIssues.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testLegacySearchIssues.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GitTree.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GitTree.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetFiles.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetFiles.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Logging.testLoggingWithOAuthAuthentication.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Logging.testLoggingWithOAuthAuthentication.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testGetLabels.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testGetLabels.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testMergeWithMessage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testMergeWithMessage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testAttributes.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testAttributes.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Team.testEditWithoutArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Team.testEditWithoutArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchReposExplicitPagination.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchReposExplicitPagination.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testSliceIndexingInFirstPage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testSliceIndexingInFirstPage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetAuthorizations.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetAuthorizations.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Milestone.testEditWithAllParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Milestone.testEditWithAllParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testEditWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testEditWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Team.testRepos.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Team.testRepos.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testDeleteAndSetLabels.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testDeleteAndSetLabels.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Logging.testLoggingWithBaseUrl.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Logging.testLoggingWithBaseUrl.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateRepositoryWithAutoInit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateRepositoryWithAutoInit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetContents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetContents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue54.testConversion.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue54.testConversion.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetGitRefWithIssue102Reverted.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetGitRefWithIssue102Reverted.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreatePullFromIssue.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreatePullFromIssue.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateKey.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateKey.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetCommits.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetCommits.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue87.testCreateIssueWithEscapedPercentInTitle.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue87.testCreateIssueWithEscapedPercentInTitle.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetGitTreeWithRecursive.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetGitTreeWithRecursive.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateIssueWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateIssueWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetMilestones.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetMilestones.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testCreateGistWithoutDescription.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testCreateGistWithoutDescription.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Gist.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Gist.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateMilestone.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateMilestone.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testAddLabelToIssue.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testAddLabelToIssue.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Event.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Event.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/UserKey.testEditWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/UserKey.testEditWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testGetThirdPage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testGetThirdPage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetPublicMembers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetPublicMembers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GistComment.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GistComment.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetStargazers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetStargazers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testEditWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testEditWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/CommitComment.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/CommitComment.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetPulls.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetPulls.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testDelete.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testDelete.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Download.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Download.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetFollowing.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetFollowing.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateAuthorizationWithoutArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateAuthorizationWithoutArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateIssue.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateIssue.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Tag.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Tag.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testSeveralIterations.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testSeveralIterations.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetOrganizationEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetOrganizationEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testSliceIndexingUntilEnd.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testSliceIndexingUntilEnd.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetRepos.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetRepos.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetGitRef.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetGitRef.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GitRef.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GitRef.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testEditResetMilestone.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testEditResetMilestone.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetForks.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetForks.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Logging.testLoggingWithBasicAuthentication.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Logging.testLoggingWithBasicAuthentication.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateTeam.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateTeam.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testEditWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testEditWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetFollowers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetFollowers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testGetEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testGetEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitCommitWithParents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitCommitWithParents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Authorization.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Authorization.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetIssuesWithArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetIssuesWithArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testEditWithAllParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testEditWithAllParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitBlob.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitBlob.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Team.testEditWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Team.testEditWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/RepositoryKey.testEditWithoutParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/RepositoryKey.testEditWithoutParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue80.testIgnoreHttpsFromGithubEnterpriseWithPort.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue80.testIgnoreHttpsFromGithubEnterpriseWithPort.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Enterprise.testSpecificPort.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Enterprise.testSpecificPort.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetGists.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetGists.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateRepositoryWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateRepositoryWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GitRef.testEdit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GitRef.testEdit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetComments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetComments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetIssueComments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetIssueComments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GitRef.testEditWithForce.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GitRef.testEditWithForce.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Team.testMembers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Team.testMembers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue33.testClosedIssues.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue33.testClosedIssues.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetDownloads.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetDownloads.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Authentication.testSecretKeyAuthentication.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Authentication.testSecretKeyAuthentication.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testMembers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testMembers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue33.testOpenIssues.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue33.testOpenIssues.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateRepoWithMinimalArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateRepoWithMinimalArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Authorization.testEdit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Authorization.testEdit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateDownloadWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateDownloadWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetMilestonesWithArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetMilestonesWithArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateCommentOnFileLine.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateCommentOnFileLine.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTagWithAllArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTagWithAllArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Gist.testEditWithAllParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Gist.testEditWithAllParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/RepositoryKey.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/RepositoryKey.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Hook.testEditWithMinimalParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Hook.testEditWithMinimalParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testSetIssueLabels.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testSetIssueLabels.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchRepos.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchRepos.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testGetReposWithType.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testGetReposWithType.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitTag.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitTag.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetGitRefs.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetGitRefs.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetPublicEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetPublicEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testEditWithoutArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testEditWithoutArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue87.testCreateIssueWithPercentInTitle.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue87.testCreateIssueWithPercentInTitle.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetCommits.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetCommits.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetKeys.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetKeys.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GistComment.testEdit.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GistComment.testEdit.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateFork.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateFork.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateComment.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateComment.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testSearchIssues.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testSearchIssues.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testIssueGetLabels.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testIssueGetLabels.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/CommitStatus.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/CommitStatus.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Exceptions.testInvalidInput.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Exceptions.testInvalidInput.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue87.testCreateIssueWithPercentInBody.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue87.testCreateIssueWithPercentInBody.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateHookWithMinimalParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateHookWithMinimalParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetRepo.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetRepo.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testEditWithoutArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testEditWithoutArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue.testCreateComment.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue.testCreateComment.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetIssuesEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetIssuesEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testCreateGistWithoutDescription.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testCreateGistWithoutDescription.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetArchiveLink.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetArchiveLink.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetRepos.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetRepos.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Commit.testCreateStatusWithAllParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Commit.testCreateStatusWithAllParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testGetFirstPage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testGetFirstPage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue50.testCreateLabel.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue50.testCreateLabel.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testStarring.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testStarring.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testGetHooks.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testGetHooks.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchUsersPagination.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchUsersPagination.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue33.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue33.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetBranch.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetBranch.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testInterruptedIteration.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testInterruptedIteration.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Gist.testEditWithoutParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Gist.testEditWithoutParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetOrgs.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetOrgs.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateDownloadWithMinimalArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateDownloadWithMinimalArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Branch.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Branch.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetPullsWithArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetPullsWithArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateHookWithAllParameters.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateHookWithAllParameters.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequestFile.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequestFile.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testCreateFork.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testCreateFork.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateGitRef.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateGitRef.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testMergeWithCommitMessage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testMergeWithCommitMessage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetPublicReceivedEvents.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetPublicReceivedEvents.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PaginatedList.testIntIndexingInFirstPage.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PaginatedList.testIntIndexingInFirstPage.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testGetStarredGists.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testGetStarredGists.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Markdown.testRenderMarkdown.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Markdown.testRenderMarkdown.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Organization.testPublicMembers.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Organization.testPublicMembers.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testMerge.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testMerge.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testSubscriptions.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testSubscriptions.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/GitCommit.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/GitCommit.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Authentication.testUserAgent.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Authentication.testUserAgent.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/PullRequest.testGetIssueComment.txt` & `PyGithub-1.9.1/github/tests/ReplayData/PullRequest.testGetIssueComment.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/AuthenticatedUser.testEmails.txt` & `PyGithub-1.9.1/github/tests/ReplayData/AuthenticatedUser.testEmails.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/NamedUser.testGetRepos.txt` & `PyGithub-1.9.1/github/tests/ReplayData/NamedUser.testGetRepos.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Enterprise.testHttps.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Enterprise.testHttps.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testCreateLabel.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testCreateLabel.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Repository.testGetCommitsWithArguments.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Repository.testGetCommitsWithArguments.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Team.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Team.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Logging.testLoggingWithoutAuthentication.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Logging.testLoggingWithoutAuthentication.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Issue54.setUp.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Issue54.setUp.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/ReplayData/Github.testLegacySearchUserByEmail.txt` & `PyGithub-1.9.1/github/tests/ReplayData/Github.testLegacySearchUserByEmail.txt`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/GitRef.py` & `PyGithub-1.9.1/github/tests/GitRef.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/RepositoryKey.py` & `PyGithub-1.9.1/github/tests/RepositoryKey.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Hook.py` & `PyGithub-1.9.1/github/tests/Hook.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/CommitComment.py` & `PyGithub-1.9.1/github/tests/CommitComment.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Framework.py` & `PyGithub-1.9.1/github/tests/Framework.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Tag.py` & `PyGithub-1.9.1/github/tests/Tag.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/PaginatedList.py` & `PyGithub-1.9.1/github/tests/PaginatedList.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/__init__.py` & `PyGithub-1.9.1/github/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Logging_.py` & `PyGithub-1.9.1/github/tests/Logging_.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/PullRequestFile.py` & `PyGithub-1.9.1/github/tests/PullRequestFile.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Issue33.py` & `PyGithub-1.9.1/github/tests/Issue33.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Download.py` & `PyGithub-1.9.1/github/tests/Download.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Label.py` & `PyGithub-1.9.1/github/tests/Label.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/CommitStatus.py` & `PyGithub-1.9.1/github/tests/CommitStatus.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Team.py` & `PyGithub-1.9.1/github/tests/Team.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Organization.py` & `PyGithub-1.9.1/github/tests/Organization.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Gist.py` & `PyGithub-1.9.1/github/tests/Gist.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Milestone.py` & `PyGithub-1.9.1/github/tests/Milestone.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Repository.py` & `PyGithub-1.9.1/github/tests/Repository.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Github_.py` & `PyGithub-1.9.1/github/tests/Github_.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Markdown.py` & `PyGithub-1.9.1/github/tests/Markdown.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/RateLimiting.py` & `PyGithub-1.9.1/github/tests/RateLimiting.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/PullRequest.py` & `PyGithub-1.9.1/github/tests/PullRequest.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/IssueEvent.py` & `PyGithub-1.9.1/github/tests/IssueEvent.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/Issue.py` & `PyGithub-1.9.1/github/tests/Issue.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/GistComment.py` & `PyGithub-1.9.1/github/tests/GistComment.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/tests/UserKey.py` & `PyGithub-1.9.1/github/tests/UserKey.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/HookResponse.py` & `PyGithub-1.9.1/github/HookResponse.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def _initAttributes(self):
         self._code = GithubObject.NotSet
         self._message = GithubObject.NotSet
         self._status = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "code" in attributes:  # pragma no branch
-            assert attributes["code"] is None or isinstance(attributes["code"], int), attributes["code"]
+            assert attributes["code"] is None or isinstance(attributes["code"], (int, long)), attributes["code"]
             self._code = attributes["code"]
         if "message" in attributes:  # pragma no branch
             assert attributes["message"] is None or isinstance(attributes["message"], (str, unicode)), attributes["message"]
             self._message = attributes["message"]
         if "status" in attributes:  # pragma no branch
             assert attributes["status"] is None or isinstance(attributes["status"], (str, unicode)), attributes["status"]
             self._status = attributes["status"]
```

### Comparing `PyGithub-1.9.0/github/Gist.py` & `PyGithub-1.9.1/github/Gist.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             self.url,
             None,
             post_parameters
         )
         self._useAttributes(data)
 
     def get_comment(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/comments/" + str(id),
             None,
             None
         )
         return GistComment.GistComment(self._requester, data, completed=True)
@@ -204,15 +204,15 @@
         self._public = GithubObject.NotSet
         self._updated_at = GithubObject.NotSet
         self._url = GithubObject.NotSet
         self._user = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "comments" in attributes:  # pragma no branch
-            assert attributes["comments"] is None or isinstance(attributes["comments"], int), attributes["comments"]
+            assert attributes["comments"] is None or isinstance(attributes["comments"], (int, long)), attributes["comments"]
             self._comments = attributes["comments"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "description" in attributes:  # pragma no branch
             assert attributes["description"] is None or isinstance(attributes["description"], (str, unicode)), attributes["description"]
             self._description = attributes["description"]
```

### Comparing `PyGithub-1.9.0/github/Milestone.py` & `PyGithub-1.9.1/github/Milestone.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,36 +131,36 @@
         self._open_issues = GithubObject.NotSet
         self._state = GithubObject.NotSet
         self._title = GithubObject.NotSet
         self._url = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "closed_issues" in attributes:  # pragma no branch
-            assert attributes["closed_issues"] is None or isinstance(attributes["closed_issues"], int), attributes["closed_issues"]
+            assert attributes["closed_issues"] is None or isinstance(attributes["closed_issues"], (int, long)), attributes["closed_issues"]
             self._closed_issues = attributes["closed_issues"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "creator" in attributes:  # pragma no branch
             assert attributes["creator"] is None or isinstance(attributes["creator"], dict), attributes["creator"]
             self._creator = None if attributes["creator"] is None else NamedUser.NamedUser(self._requester, attributes["creator"], completed=False)
         if "description" in attributes:  # pragma no branch
             assert attributes["description"] is None or isinstance(attributes["description"], (str, unicode)), attributes["description"]
             self._description = attributes["description"]
         if "due_on" in attributes:  # pragma no branch
             assert attributes["due_on"] is None or isinstance(attributes["due_on"], (str, unicode)), attributes["due_on"]
             self._due_on = self._parseDatetime(attributes["due_on"])
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "number" in attributes:  # pragma no branch
-            assert attributes["number"] is None or isinstance(attributes["number"], int), attributes["number"]
+            assert attributes["number"] is None or isinstance(attributes["number"], (int, long)), attributes["number"]
             self._number = attributes["number"]
         if "open_issues" in attributes:  # pragma no branch
-            assert attributes["open_issues"] is None or isinstance(attributes["open_issues"], int), attributes["open_issues"]
+            assert attributes["open_issues"] is None or isinstance(attributes["open_issues"], (int, long)), attributes["open_issues"]
             self._open_issues = attributes["open_issues"]
         if "state" in attributes:  # pragma no branch
             assert attributes["state"] is None or isinstance(attributes["state"], (str, unicode)), attributes["state"]
             self._state = attributes["state"]
         if "title" in attributes:  # pragma no branch
             assert attributes["title"] is None or isinstance(attributes["title"], (str, unicode)), attributes["title"]
             self._title = attributes["title"]
```

### Comparing `PyGithub-1.9.0/github/Repository.py` & `PyGithub-1.9.1/github/Repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             None,
             None
         )
         return Comparison.Comparison(self._requester, data, completed=True)
 
     def create_download(self, name, size, description=GithubObject.NotSet, content_type=GithubObject.NotSet):
         assert isinstance(name, (str, unicode)), name
-        assert isinstance(size, int), size
+        assert isinstance(size, (int, long)), size
         assert description is GithubObject.NotSet or isinstance(description, (str, unicode)), description
         assert content_type is GithubObject.NotSet or isinstance(content_type, (str, unicode)), content_type
         post_parameters = {
             "name": name,
             "size": size,
         }
         if description is not GithubObject.NotSet:
@@ -546,15 +546,15 @@
             NamedUser.NamedUser,
             self._requester,
             self.url + "/collaborators",
             None
         )
 
     def get_comment(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/comments/" + str(id),
             None,
             None
         )
         return CommitComment.CommitComment(self._requester, data, completed=True)
@@ -607,15 +607,15 @@
             NamedUser.NamedUser,
             self._requester,
             self.url + "/contributors",
             None
         )
 
     def get_download(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/downloads/" + str(id),
             None,
             None
         )
         return Download.Download(self._requester, data, completed=True)
@@ -706,15 +706,15 @@
             self.url + "/git/trees/" + sha,
             url_parameters,
             None
         )
         return GitTree.GitTree(self._requester, data, completed=True)
 
     def get_hook(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/hooks/" + str(id),
             None,
             None
         )
         return Hook.Hook(self._requester, data, completed=True)
@@ -724,15 +724,15 @@
             Hook.Hook,
             self._requester,
             self.url + "/hooks",
             None
         )
 
     def get_issue(self, number):
-        assert isinstance(number, int), number
+        assert isinstance(number, (int, long)), number
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/issues/" + str(number),
             None,
             None
         )
         return Issue.Issue(self._requester, data, completed=True)
@@ -773,15 +773,15 @@
             Issue.Issue,
             self._requester,
             self.url + "/issues",
             url_parameters
         )
 
     def get_issues_event(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/issues/events/" + str(id),
             None,
             None
         )
         return IssueEvent.IssueEvent(self._requester, data, completed=True)
@@ -791,15 +791,15 @@
             IssueEvent.IssueEvent,
             self._requester,
             self.url + "/issues/events",
             None
         )
 
     def get_key(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/keys/" + str(id),
             None,
             None
         )
         return RepositoryKey.RepositoryKey(self._requester, data, completed=True, repoUrl=self._url)
@@ -836,15 +836,15 @@
             self.url + "/languages",
             None,
             None
         )
         return data
 
     def get_milestone(self, number):
-        assert isinstance(number, int), number
+        assert isinstance(number, (int, long)), number
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/milestones/" + str(number),
             None,
             None
         )
         return Milestone.Milestone(self._requester, data, completed=True)
@@ -872,15 +872,15 @@
             Event.Event,
             self._requester,
             "/networks/" + self.owner.login + "/" + self.name + "/events",
             None
         )
 
     def get_pull(self, number):
-        assert isinstance(number, int), number
+        assert isinstance(number, (int, long)), number
         headers, data = self._requester.requestAndCheck(
             "GET",
             self.url + "/pulls/" + str(number),
             None,
             None
         )
         return PullRequest.PullRequest(self._requester, data, completed=True)
@@ -1056,15 +1056,15 @@
         if "description" in attributes:  # pragma no branch
             assert attributes["description"] is None or isinstance(attributes["description"], (str, unicode)), attributes["description"]
             self._description = attributes["description"]
         if "fork" in attributes:  # pragma no branch
             assert attributes["fork"] is None or isinstance(attributes["fork"], bool), attributes["fork"]
             self._fork = attributes["fork"]
         if "forks" in attributes:  # pragma no branch
-            assert attributes["forks"] is None or isinstance(attributes["forks"], int), attributes["forks"]
+            assert attributes["forks"] is None or isinstance(attributes["forks"], (int, long)), attributes["forks"]
             self._forks = attributes["forks"]
         if "full_name" in attributes:  # pragma no branch
             assert attributes["full_name"] is None or isinstance(attributes["full_name"], (str, unicode)), attributes["full_name"]
             self._full_name = attributes["full_name"]
         if "git_url" in attributes:  # pragma no branch
             assert attributes["git_url"] is None or isinstance(attributes["git_url"], (str, unicode)), attributes["git_url"]
             self._git_url = attributes["git_url"]
@@ -1080,27 +1080,27 @@
         if "homepage" in attributes:  # pragma no branch
             assert attributes["homepage"] is None or isinstance(attributes["homepage"], (str, unicode)), attributes["homepage"]
             self._homepage = attributes["homepage"]
         if "html_url" in attributes:  # pragma no branch
             assert attributes["html_url"] is None or isinstance(attributes["html_url"], (str, unicode)), attributes["html_url"]
             self._html_url = attributes["html_url"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "language" in attributes:  # pragma no branch
             assert attributes["language"] is None or isinstance(attributes["language"], (str, unicode)), attributes["language"]
             self._language = attributes["language"]
         if "master_branch" in attributes:  # pragma no branch
             assert attributes["master_branch"] is None or isinstance(attributes["master_branch"], (str, unicode)), attributes["master_branch"]
             self._master_branch = attributes["master_branch"]
         if "name" in attributes:  # pragma no branch
             assert attributes["name"] is None or isinstance(attributes["name"], (str, unicode)), attributes["name"]
             self._name = attributes["name"]
         if "open_issues" in attributes:  # pragma no branch
-            assert attributes["open_issues"] is None or isinstance(attributes["open_issues"], int), attributes["open_issues"]
+            assert attributes["open_issues"] is None or isinstance(attributes["open_issues"], (int, long)), attributes["open_issues"]
             self._open_issues = attributes["open_issues"]
         if "organization" in attributes:  # pragma no branch
             assert attributes["organization"] is None or isinstance(attributes["organization"], dict), attributes["organization"]
             self._organization = None if attributes["organization"] is None else Organization.Organization(self._requester, attributes["organization"], completed=False)
         if "owner" in attributes:  # pragma no branch
             assert attributes["owner"] is None or isinstance(attributes["owner"], dict), attributes["owner"]
             self._owner = None if attributes["owner"] is None else NamedUser.NamedUser(self._requester, attributes["owner"], completed=False)
@@ -1113,15 +1113,15 @@
         if "private" in attributes:  # pragma no branch
             assert attributes["private"] is None or isinstance(attributes["private"], bool), attributes["private"]
             self._private = attributes["private"]
         if "pushed_at" in attributes:  # pragma no branch
             assert attributes["pushed_at"] is None or isinstance(attributes["pushed_at"], (str, unicode)), attributes["pushed_at"]
             self._pushed_at = self._parseDatetime(attributes["pushed_at"])
         if "size" in attributes:  # pragma no branch
-            assert attributes["size"] is None or isinstance(attributes["size"], int), attributes["size"]
+            assert attributes["size"] is None or isinstance(attributes["size"], (int, long)), attributes["size"]
             self._size = attributes["size"]
         if "source" in attributes:  # pragma no branch
             assert attributes["source"] is None or isinstance(attributes["source"], dict), attributes["source"]
             self._source = None if attributes["source"] is None else Repository(self._requester, attributes["source"], completed=False)
         if "ssh_url" in attributes:  # pragma no branch
             assert attributes["ssh_url"] is None or isinstance(attributes["ssh_url"], (str, unicode)), attributes["ssh_url"]
             self._ssh_url = attributes["ssh_url"]
@@ -1131,9 +1131,9 @@
         if "updated_at" in attributes:  # pragma no branch
             assert attributes["updated_at"] is None or isinstance(attributes["updated_at"], (str, unicode)), attributes["updated_at"]
             self._updated_at = self._parseDatetime(attributes["updated_at"])
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
         if "watchers" in attributes:  # pragma no branch
-            assert attributes["watchers"] is None or isinstance(attributes["watchers"], int), attributes["watchers"]
+            assert attributes["watchers"] is None or isinstance(attributes["watchers"], (int, long)), attributes["watchers"]
             self._watchers = attributes["watchers"]
```

### Comparing `PyGithub-1.9.0/github/GitObject.py` & `PyGithub-1.9.1/github/GitObject.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/IssuePullRequest.py` & `PyGithub-1.9.1/github/IssuePullRequest.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Permissions.py` & `PyGithub-1.9.1/github/Permissions.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/Requester.py` & `PyGithub-1.9.1/github/Requester.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/PullRequestMergeStatus.py` & `PyGithub-1.9.1/github/PullRequestMergeStatus.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/PullRequest.py` & `PyGithub-1.9.1/github/PullRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     def create_comment(self, body, commit_id, path, position):
         return self.create_review_comment(body, commit_id, path, position)
 
     def create_review_comment(self, body, commit_id, path, position):
         assert isinstance(body, (str, unicode)), body
         assert isinstance(commit_id, Commit.Commit), commit_id
         assert isinstance(path, (str, unicode)), path
-        assert isinstance(position, int), position
+        assert isinstance(position, (int, long)), position
         post_parameters = {
             "body": body,
             "commit_id": commit_id._identity,
             "path": path,
             "position": position,
         }
         headers, data = self._requester.requestAndCheck(
@@ -215,15 +215,15 @@
         )
         self._useAttributes(data)
 
     def get_comment(self, id):
         return self.get_review_comment(id)
 
     def get_review_comment(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self._parentUrl(self.url) + "/comments/" + str(id),
             None,
             None
         )
         return PullRequestComment.PullRequestComment(self._requester, data, completed=True)
@@ -252,15 +252,15 @@
             File.File,
             self._requester,
             self.url + "/files",
             None
         )
 
     def get_issue_comment(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self._parentUrl(self._parentUrl(self.url)) + "/issues/comments/" + str(id),
             None,
             None
         )
         return IssueComment.IssueComment(self._requester, data, completed=True)
@@ -322,54 +322,54 @@
         self._title = GithubObject.NotSet
         self._updated_at = GithubObject.NotSet
         self._url = GithubObject.NotSet
         self._user = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "additions" in attributes:  # pragma no branch
-            assert attributes["additions"] is None or isinstance(attributes["additions"], int), attributes["additions"]
+            assert attributes["additions"] is None or isinstance(attributes["additions"], (int, long)), attributes["additions"]
             self._additions = attributes["additions"]
         if "assignee" in attributes:  # pragma no branch
             assert attributes["assignee"] is None or isinstance(attributes["assignee"], dict), attributes["assignee"]
             self._assignee = None if attributes["assignee"] is None else NamedUser.NamedUser(self._requester, attributes["assignee"], completed=False)
         if "base" in attributes:  # pragma no branch
             assert attributes["base"] is None or isinstance(attributes["base"], dict), attributes["base"]
             self._base = None if attributes["base"] is None else PullRequestPart.PullRequestPart(self._requester, attributes["base"], completed=False)
         if "body" in attributes:  # pragma no branch
             assert attributes["body"] is None or isinstance(attributes["body"], (str, unicode)), attributes["body"]
             self._body = attributes["body"]
         if "changed_files" in attributes:  # pragma no branch
-            assert attributes["changed_files"] is None or isinstance(attributes["changed_files"], int), attributes["changed_files"]
+            assert attributes["changed_files"] is None or isinstance(attributes["changed_files"], (int, long)), attributes["changed_files"]
             self._changed_files = attributes["changed_files"]
         if "closed_at" in attributes:  # pragma no branch
             assert attributes["closed_at"] is None or isinstance(attributes["closed_at"], (str, unicode)), attributes["closed_at"]
             self._closed_at = self._parseDatetime(attributes["closed_at"])
         if "comments" in attributes:  # pragma no branch
-            assert attributes["comments"] is None or isinstance(attributes["comments"], int), attributes["comments"]
+            assert attributes["comments"] is None or isinstance(attributes["comments"], (int, long)), attributes["comments"]
             self._comments = attributes["comments"]
         if "commits" in attributes:  # pragma no branch
-            assert attributes["commits"] is None or isinstance(attributes["commits"], int), attributes["commits"]
+            assert attributes["commits"] is None or isinstance(attributes["commits"], (int, long)), attributes["commits"]
             self._commits = attributes["commits"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "deletions" in attributes:  # pragma no branch
-            assert attributes["deletions"] is None or isinstance(attributes["deletions"], int), attributes["deletions"]
+            assert attributes["deletions"] is None or isinstance(attributes["deletions"], (int, long)), attributes["deletions"]
             self._deletions = attributes["deletions"]
         if "diff_url" in attributes:  # pragma no branch
             assert attributes["diff_url"] is None or isinstance(attributes["diff_url"], (str, unicode)), attributes["diff_url"]
             self._diff_url = attributes["diff_url"]
         if "head" in attributes:  # pragma no branch
             assert attributes["head"] is None or isinstance(attributes["head"], dict), attributes["head"]
             self._head = None if attributes["head"] is None else PullRequestPart.PullRequestPart(self._requester, attributes["head"], completed=False)
         if "html_url" in attributes:  # pragma no branch
             assert attributes["html_url"] is None or isinstance(attributes["html_url"], (str, unicode)), attributes["html_url"]
             self._html_url = attributes["html_url"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "issue_url" in attributes:  # pragma no branch
             assert attributes["issue_url"] is None or isinstance(attributes["issue_url"], (str, unicode)), attributes["issue_url"]
             self._issue_url = attributes["issue_url"]
         if "mergeable" in attributes:  # pragma no branch
             assert attributes["mergeable"] is None or isinstance(attributes["mergeable"], bool), attributes["mergeable"]
             self._mergeable = attributes["mergeable"]
@@ -379,21 +379,21 @@
         if "merged_at" in attributes:  # pragma no branch
             assert attributes["merged_at"] is None or isinstance(attributes["merged_at"], (str, unicode)), attributes["merged_at"]
             self._merged_at = self._parseDatetime(attributes["merged_at"])
         if "merged_by" in attributes:  # pragma no branch
             assert attributes["merged_by"] is None or isinstance(attributes["merged_by"], dict), attributes["merged_by"]
             self._merged_by = None if attributes["merged_by"] is None else NamedUser.NamedUser(self._requester, attributes["merged_by"], completed=False)
         if "number" in attributes:  # pragma no branch
-            assert attributes["number"] is None or isinstance(attributes["number"], int), attributes["number"]
+            assert attributes["number"] is None or isinstance(attributes["number"], (int, long)), attributes["number"]
             self._number = attributes["number"]
         if "patch_url" in attributes:  # pragma no branch
             assert attributes["patch_url"] is None or isinstance(attributes["patch_url"], (str, unicode)), attributes["patch_url"]
             self._patch_url = attributes["patch_url"]
         if "review_comments" in attributes:  # pragma no branch
-            assert attributes["review_comments"] is None or isinstance(attributes["review_comments"], int), attributes["review_comments"]
+            assert attributes["review_comments"] is None or isinstance(attributes["review_comments"], (int, long)), attributes["review_comments"]
             self._review_comments = attributes["review_comments"]
         if "state" in attributes:  # pragma no branch
             assert attributes["state"] is None or isinstance(attributes["state"], (str, unicode)), attributes["state"]
             self._state = attributes["state"]
         if "title" in attributes:  # pragma no branch
             assert attributes["title"] is None or isinstance(attributes["title"], (str, unicode)), attributes["title"]
             self._title = attributes["title"]
```

### Comparing `PyGithub-1.9.0/github/HookDescription.py` & `PyGithub-1.9.1/github/HookDescription.py`

 * *Files identical despite different names*

### Comparing `PyGithub-1.9.0/github/IssueEvent.py` & `PyGithub-1.9.1/github/IssueEvent.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "event" in attributes:  # pragma no branch
             assert attributes["event"] is None or isinstance(attributes["event"], (str, unicode)), attributes["event"]
             self._event = attributes["event"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "issue" in attributes:  # pragma no branch
             assert attributes["issue"] is None or isinstance(attributes["issue"], dict), attributes["issue"]
             self._issue = None if attributes["issue"] is None else Issue.Issue(self._requester, attributes["issue"], completed=False)
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/Issue.py` & `PyGithub-1.9.1/github/Issue.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             self.url,
             None,
             post_parameters
         )
         self._useAttributes(data)
 
     def get_comment(self, id):
-        assert isinstance(id, int), id
+        assert isinstance(id, (int, long)), id
         headers, data = self._requester.requestAndCheck(
             "GET",
             self._parentUrl(self.url) + "/comments/" + str(id),
             None,
             None
         )
         return IssueComment.IssueComment(self._requester, data, completed=True)
@@ -262,36 +262,36 @@
         if "closed_at" in attributes:  # pragma no branch
             assert attributes["closed_at"] is None or isinstance(attributes["closed_at"], (str, unicode)), attributes["closed_at"]
             self._closed_at = self._parseDatetime(attributes["closed_at"])
         if "closed_by" in attributes:  # pragma no branch
             assert attributes["closed_by"] is None or isinstance(attributes["closed_by"], dict), attributes["closed_by"]
             self._closed_by = None if attributes["closed_by"] is None else NamedUser.NamedUser(self._requester, attributes["closed_by"], completed=False)
         if "comments" in attributes:  # pragma no branch
-            assert attributes["comments"] is None or isinstance(attributes["comments"], int), attributes["comments"]
+            assert attributes["comments"] is None or isinstance(attributes["comments"], (int, long)), attributes["comments"]
             self._comments = attributes["comments"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "html_url" in attributes:  # pragma no branch
             assert attributes["html_url"] is None or isinstance(attributes["html_url"], (str, unicode)), attributes["html_url"]
             self._html_url = attributes["html_url"]
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "labels" in attributes:  # pragma no branch
             assert attributes["labels"] is None or all(isinstance(element, dict) for element in attributes["labels"]), attributes["labels"]
             self._labels = None if attributes["labels"] is None else [
                 Label.Label(self._requester, element, completed=False)
                 for element in attributes["labels"]
             ]
         if "milestone" in attributes:  # pragma no branch
             assert attributes["milestone"] is None or isinstance(attributes["milestone"], dict), attributes["milestone"]
             self._milestone = None if attributes["milestone"] is None else Milestone.Milestone(self._requester, attributes["milestone"], completed=False)
         if "number" in attributes:  # pragma no branch
-            assert attributes["number"] is None or isinstance(attributes["number"], int), attributes["number"]
+            assert attributes["number"] is None or isinstance(attributes["number"], (int, long)), attributes["number"]
             self._number = attributes["number"]
         if "pull_request" in attributes:  # pragma no branch
             assert attributes["pull_request"] is None or isinstance(attributes["pull_request"], dict), attributes["pull_request"]
             self._pull_request = None if attributes["pull_request"] is None else IssuePullRequest.IssuePullRequest(self._requester, attributes["pull_request"], completed=False)
         if "repository" in attributes:  # pragma no branch
             assert attributes["repository"] is None or isinstance(attributes["repository"], dict), attributes["repository"]
             self._repository = None if attributes["repository"] is None else Repository.Repository(self._requester, attributes["repository"], completed=False)
```

### Comparing `PyGithub-1.9.0/github/GistComment.py` & `PyGithub-1.9.1/github/GistComment.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         if "body" in attributes:  # pragma no branch
             assert attributes["body"] is None or isinstance(attributes["body"], (str, unicode)), attributes["body"]
             self._body = attributes["body"]
         if "created_at" in attributes:  # pragma no branch
             assert attributes["created_at"] is None or isinstance(attributes["created_at"], (str, unicode)), attributes["created_at"]
             self._created_at = self._parseDatetime(attributes["created_at"])
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "updated_at" in attributes:  # pragma no branch
             assert attributes["updated_at"] is None or isinstance(attributes["updated_at"], (str, unicode)), attributes["updated_at"]
             self._updated_at = self._parseDatetime(attributes["updated_at"])
         if "url" in attributes:  # pragma no branch
             assert attributes["url"] is None or isinstance(attributes["url"], (str, unicode)), attributes["url"]
             self._url = attributes["url"]
```

### Comparing `PyGithub-1.9.0/github/UserKey.py` & `PyGithub-1.9.1/github/UserKey.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self._key = GithubObject.NotSet
         self._title = GithubObject.NotSet
         self._url = GithubObject.NotSet
         self._verified = GithubObject.NotSet
 
     def _useAttributes(self, attributes):
         if "id" in attributes:  # pragma no branch
-            assert attributes["id"] is None or isinstance(attributes["id"], int), attributes["id"]
+            assert attributes["id"] is None or isinstance(attributes["id"], (int, long)), attributes["id"]
             self._id = attributes["id"]
         if "key" in attributes:  # pragma no branch
             assert attributes["key"] is None or isinstance(attributes["key"], (str, unicode)), attributes["key"]
             self._key = attributes["key"]
         if "title" in attributes:  # pragma no branch
             assert attributes["title"] is None or isinstance(attributes["title"], (str, unicode)), attributes["title"]
             self._title = attributes["title"]
```

### Comparing `PyGithub-1.9.0/github/Legacy.py` & `PyGithub-1.9.1/github/Legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def _fetchNextPage(self):
         page = self.__nextPage
         self.__nextPage += 1
         return self.get_page(page)
 
     def get_page(self, page):
-        assert isinstance(page, int), page
+        assert isinstance(page, (int, long)), page
         args = dict(self.__args)
         if page != 0:
             args["start_page"] = page + 1
         headers, data = self.__requester.requestAndCheck(
             "GET",
             self.__url,
             args,
```

