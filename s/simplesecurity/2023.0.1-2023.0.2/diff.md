# Comparing `tmp/simplesecurity-2023.0.1.tar.gz` & `tmp/simplesecurity-2023.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesecurity-2023.0.1.tar", max compression
+gzip compressed data, was "simplesecurity-2023.0.2.tar", max compression
```

## Comparing `simplesecurity-2023.0.1.tar` & `simplesecurity-2023.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1080 2023-01-01 17:54:43.116685 simplesecurity-2023.0.1/LICENSE.md
--rw-r--r--   0        0        0     2441 2023-06-27 18:01:21.037624 simplesecurity-2023.0.1/pyproject.toml
--rw-r--r--   0        0        0     9940 2023-06-27 15:36:41.759046 simplesecurity-2023.0.1/README.md
--rw-r--r--   0        0        0     4757 2023-06-27 18:01:01.766192 simplesecurity-2023.0.1/simplesecurity/__init__.py
--rw-r--r--   0        0        0      116 2023-06-27 18:01:01.767192 simplesecurity-2023.0.1/simplesecurity/__main__.py
--rw-r--r--   0        0        0     1041 2023-06-27 18:01:01.760820 simplesecurity-2023.0.1/simplesecurity/excluded.py
--rw-r--r--   0        0        0     2712 2023-06-27 18:01:01.761819 simplesecurity-2023.0.1/simplesecurity/filter.py
--rw-r--r--   0        0        0     8956 2023-06-27 18:01:01.762818 simplesecurity-2023.0.1/simplesecurity/formatter.py
--rw-r--r--   0        0        0      953 2023-06-27 18:01:01.763582 simplesecurity-2023.0.1/simplesecurity/level.py
--rw-r--r--   0        0        0     9748 2023-06-27 18:01:01.765192 simplesecurity-2023.0.1/simplesecurity/plugins.py
--rw-r--r--   0        0        0   160087 2023-01-01 17:54:43.133800 simplesecurity-2023.0.1/simplesecurity/semgrep_sec.yaml
--rw-r--r--   0        0        0      715 2023-06-27 18:01:01.765192 simplesecurity-2023.0.1/simplesecurity/types.py
--rw-r--r--   0        0        0    11308 1970-01-01 00:00:00.000000 simplesecurity-2023.0.1/setup.py
--rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 simplesecurity-2023.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-01-01 17:54:43.116685 simplesecurity-2023.0.2/LICENSE.md
+-rw-r--r--   0        0        0     2441 2023-06-27 19:21:19.772901 simplesecurity-2023.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9940 2023-06-27 15:36:41.759046 simplesecurity-2023.0.2/README.md
+-rw-r--r--   0        0        0     4757 2023-06-27 19:21:07.575305 simplesecurity-2023.0.2/simplesecurity/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-27 19:21:07.576265 simplesecurity-2023.0.2/simplesecurity/__main__.py
+-rw-r--r--   0        0        0     1041 2023-06-27 19:21:07.567162 simplesecurity-2023.0.2/simplesecurity/excluded.py
+-rw-r--r--   0        0        0     2712 2023-06-27 19:21:07.569163 simplesecurity-2023.0.2/simplesecurity/filter.py
+-rw-r--r--   0        0        0     8956 2023-06-27 19:21:07.570304 simplesecurity-2023.0.2/simplesecurity/formatter.py
+-rw-r--r--   0        0        0      964 2023-06-27 19:21:07.571305 simplesecurity-2023.0.2/simplesecurity/level.py
+-rw-r--r--   0        0        0    10390 2023-06-27 19:21:07.573306 simplesecurity-2023.0.2/simplesecurity/plugins.py
+-rw-r--r--   0        0        0   160087 2023-01-01 17:54:43.133800 simplesecurity-2023.0.2/simplesecurity/semgrep_sec.yaml
+-rw-r--r--   0        0        0      715 2023-06-27 19:21:07.574305 simplesecurity-2023.0.2/simplesecurity/types.py
+-rw-r--r--   0        0        0    11308 1970-01-01 00:00:00.000000 simplesecurity-2023.0.2/setup.py
+-rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 simplesecurity-2023.0.2/PKG-INFO
```

### Comparing `simplesecurity-2023.0.1/LICENSE.md` & `simplesecurity-2023.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `simplesecurity-2023.0.1/pyproject.toml` & `simplesecurity-2023.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplesecurity"
-version = "2023.0.1"
+version = "2023.0.2"
 license = "mit"
 description = "Combine multiple popular python security tools and generate reports or output into different formats"
 authors = ["FredHappyface"]
 classifiers = [
 	"Environment :: Console",
 	"Environment :: MacOS X",
 	"Environment :: Win32 (MS Windows)",
```

### Comparing `simplesecurity-2023.0.1/README.md` & `simplesecurity-2023.0.2/README.md`

 * *Files identical despite different names*

### Comparing `simplesecurity-2023.0.1/simplesecurity/__init__.py` & `simplesecurity-2023.0.2/simplesecurity/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,27 +75,27 @@
 			"func": plugins.bandit,
 			"max_severity": 3,
 			"max_confidence": 3,
 			"fast": True,
 		},
 		"safety": {
 			"func": plugins.safety,
-			"max_severity": 2,
+			"max_severity": 4,
 			"max_confidence": 3,
 			"fast": True,
 		},
 		"dodgy": {
 			"func": plugins.dodgy,
 			"max_severity": 2,
 			"max_confidence": 2,
 			"fast": True,
 		},
 		"dlint": {
 			"func": plugins.dlint,
-			"max_severity": 3,
+			"max_severity": 4,
 			"max_confidence": 2,
 			"fast": True,
 		},
 		"semgrep": {
 			"func": plugins.semgrep,
 			"max_severity": 3,
 			"max_confidence": 3,
```

### Comparing `simplesecurity-2023.0.1/simplesecurity/excluded.py` & `simplesecurity-2023.0.2/simplesecurity/excluded.py`

 * *Files identical despite different names*

### Comparing `simplesecurity-2023.0.1/simplesecurity/filter.py` & `simplesecurity-2023.0.2/simplesecurity/filter.py`

 * *Files identical despite different names*

### Comparing `simplesecurity-2023.0.1/simplesecurity/formatter.py` & `simplesecurity-2023.0.2/simplesecurity/formatter.py`

 * *Files identical despite different names*

### Comparing `simplesecurity-2023.0.1/simplesecurity/level.py` & `simplesecurity-2023.0.2/simplesecurity/level.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,21 @@
 """
 from __future__ import annotations
 
 from enum import IntEnum
 
 
 class Level(IntEnum):
-	"""Levels for confidence and severity.
-
-	UNKNOWN = 0
-	LOW = 1
-	MED = 2
-	HIGH = 3
-	"""
+	"""Levels for confidence and severity."""
 
 	UNKNOWN = 0
 	LOW = 1
 	MED = 2
 	HIGH = 3
+	CRIT = 4
 
 	def __repr__(self) -> str:
 		"""__repr__ method.
 
 		Returns:
 			str: string representation of a level
 		"""
@@ -39,19 +34,21 @@
 			str: string representation of a level
 		"""
 		reprMap = {
 			Level.UNKNOWN: "Unknown",
 			Level.LOW: "Low",
 			Level.MED: "Medium",
 			Level.HIGH: "High",
+			Level.CRIT: "Critical",
 		}
 		return reprMap[self]
 
 	def toSarif(self) -> str:
 		"""Convert to sarif representation."""
 		reprMap = {
 			Level.UNKNOWN: "note",
-			Level.LOW: "warning",
+			Level.LOW: "note",
 			Level.MED: "warning",
 			Level.HIGH: "error",
+			Level.CRIT: "error",
 		}
 		return reprMap[self]
```

### Comparing `simplesecurity-2023.0.1/simplesecurity/plugins.py` & `simplesecurity-2023.0.2/simplesecurity/plugins.py`

 * *Files 21% similar despite different names*

```diff
@@ -71,23 +71,25 @@
 		file (str): file to extract evidence from
 
 	Returns:
 		list[Line]: list of lines
 	"""
 	with open(file, encoding="utf-8", errors="ignore") as fileContents:
 		start = max(desiredLine - 3, 0)
-		for line in range(start):
-			next(fileContents)
 		content = []
-		for line in range(start + 1, desiredLine + 3):
-			try:
+		try:
+			for line in range(start):
+				next(fileContents)
+			for line in range(start + 1, desiredLine + 3):
 				lineContent = next(fileContents).rstrip().replace("\t", "    ")
-			except StopIteration:
-				break
-			content.append({"selected": line == desiredLine, "line": line, "content": lineContent})
+				content.append(
+					{"selected": line == desiredLine, "line": line, "content": lineContent}
+				)
+		except StopIteration:
+			pass
 	return content
 
 
 def bandit(scanDir=".") -> list[Finding]:
 	"""Generate list of findings using bandit. requires bandit on the system path.
 
 	Params:
@@ -111,54 +113,78 @@
 	}
 	results = loads(
 		_doSysExec(
 			f"bandit -lirq -x {','.join([f'./{x}' for x in EXCLUDED])} -f json {scanDir}", False
 		)[1]
 	)["results"]
 	for result in results:
-		file = result["filename"].replace("\\", "/")
+		file = result.get("filename").replace("\\", "/")
+		resultId = result.get("test_id")
+		line = result.get("line_number")
 		findings.append(
 			{
-				"id": result["test_id"],
-				"title": f"{result['test_id']}: {result['test_name']}",
-				"description": result["issue_text"],
+				"id": resultId,
+				"title": f"{resultId}: {result.get('test_name')}",
+				"description": result.get("issue_text"),
 				"file": file,
-				"evidence": extractEvidence(result["line_number"], file),
-				"severity": levelMap[result["issue_severity"]],
-				"confidence": levelMap[result["issue_confidence"]],
-				"line": result["line_number"],
+				"evidence": extractEvidence(line, file),
+				"severity": levelMap[result.get("issue_severity")],
+				"confidence": levelMap[result.get("issue_confidence")],
+				"line": line,
 				"_other": {
-					"more_info": result["more_info"],
-					"line_range": result["line_range"],
+					"more_info": result.get("more_info"),
+					"line_range": result.get("line_range"),
 				},
 			}
 		)
 	return findings
 
 
 def _doSafetyProcessing(results: dict[str, Any]) -> list[Finding]:
 	findings = []
 	for result in results["vulnerabilities"]:
+		vulnerabilityId = result.get("vulnerability_id")
+		packageName = result.get("package_name")
+		advisory = result.get("advisory")
+
+		moreInfo = result.get("more_info_url")
+		affectedVersions = "; ".join(result.get("affected_versions"))
+
+		content = f"{packageName}, version(s)={affectedVersions}"
+		description = (
+			f"Vulnerability found in package {packageName},"
+			f"version(s)={affectedVersions}. {advisory}. More info available at {moreInfo}"
+		)
+
+		cvssv3Score = result.get("severity").get("cvssv3", {}).get("base_score", 0)
+		severity = Level.LOW
+		if cvssv3Score > 3.9:
+			severity = Level.MED
+		if cvssv3Score > 6.9:
+			severity = Level.HIGH
+		if cvssv3Score > 8.9:
+			severity = Level.CRIT
+
 		findings.append(
 			{
-				"id": result[4],
-				"title": f"{result[4]}: {result[0]}",
-				"description": result[3],
+				"id": vulnerabilityId,
+				"title": f"{vulnerabilityId}: {packageName}",
+				"description": description,
 				"file": "Project Requirements",
 				"evidence": [
 					{
 						"selected": True,
 						"line": 0,
-						"content": f"{result[0]} version={result[2]} affects{result[1]}",
+						"content": content,
 					}
 				],
-				"severity": Level.MED,
+				"severity": severity,
 				"confidence": Level.HIGH,
 				"line": "Unknown",
-				"_other": {"id": result[4], "affected": result[1]},
+				"_other": {"id": vulnerabilityId, "affectedVersions": affectedVersions},
 			}
 		)
 	return findings
 
 
 def _doPureSafety() -> dict[str, Any]:
 	safe = _doSysExec("safety check -r requirements.txt --json")[1]
@@ -223,25 +249,26 @@
 	"""
 	if _doSysExec("dodgy -h")[0] != 0:
 		raise RuntimeError("dodgy is not on the system path")
 	findings = []
 	rawResults = _doSysExec(f"dodgy {scanDir} -i {' '.join(EXCLUDED)}")[1]
 	results = loads(rawResults)["warnings"]
 	for result in results:
-		file = "./" + result["path"].replace("\\", "/")
+		file = "./" + result.get("path").replace("\\", "/")
+		message = result.get("message")
 		findings.append(
 			{
-				"id": result["code"],
-				"title": result["message"],
-				"description": result["message"],
+				"id": result.get("code"),
+				"title": message,
+				"description": message,
 				"file": file,
-				"evidence": extractEvidence(result["line"], file),
+				"evidence": extractEvidence(result.get("line"), file),
 				"severity": Level.MED,
 				"confidence": Level.MED,
-				"line": result["line"],
+				"line": result.get("line"),
 				"_other": {},
 			}
 		)
 	return findings
 
 
 def dlint(scanDir=".") -> list[Finding]:
@@ -265,37 +292,39 @@
 	)[1].splitlines(False)
 
 	jsonResults = loads("".join(results)) if len(results) > 0 else {}
 	levelMap = {
 		"info": Level.LOW,
 		"minor": Level.MED,
 		"major": Level.MED,
-		"critical": Level.HIGH,
-		"blocker": Level.HIGH,
+		"critical": Level.CRIT,
+		"blocker": Level.CRIT,
 	}
 	for filePath, scanResults in jsonResults.items():
-		for scanResult in scanResults:
+		for result in scanResults:
+			message = f"{result.get('check_name')}: " f"{result.get('description')}"
+			positions = result.get("location", {}).get("positions", {})
+			line = positions.get("begin", {}).get("line", 0)
 			findings.append(
 				{
-					"id": scanResult["check_name"],
-					"title": f"{scanResult['check_name']}: " f"{scanResult['description']}",
-					"description": f"{scanResult['check_name']}: " f"{scanResult['description']}",
+					"id": result.get("check_name"),
+					"title": message,
+					"description": message,
 					"file": filePath,
 					"evidence": extractEvidence(
-						scanResult["location"]["positions"]["begin"]["line"],
+						line,
 						filePath,
 					),
-					"severity": levelMap[scanResult["severity"]],
+					"severity": levelMap[result.get("severity")],
 					"confidence": Level.MED,
-					"line": scanResult["location"]["positions"]["begin"]["line"],
+					"line": line,
 					"_other": {
-						"col": scanResult["location"]["positions"]["begin"]["column"],
-						"start": scanResult["location"]["positions"]["begin"]["line"],
-						"end": scanResult["location"]["positions"]["end"]["line"],
-						"fingerprint": scanResult["fingerprint"],
+						"start": line,
+						"end": positions.get("end", {}).get("line", 0),
+						"fingerprint": result.get("fingerprint"),
 					},
 				}
 			)
 
 	return findings
 
 
@@ -320,28 +349,29 @@
 		_doSysExec(
 			f"semgrep -f {THISDIR}/semgrep_sec.yaml {scanDir} {' '.join(sgExclude)} "
 			"-q --json --no-rewrite-rule-ids"
 		)[1].strip()
 	)["results"]
 	levelMap = {"INFO": Level.LOW, "WARNING": Level.MED, "ERROR": Level.HIGH}
 	for result in results:
-		filePath = result["Target"].replace("\\", "/")
+		filePath = result.get("Target").replace("\\", "/")
 		file = f"{scanDir}/{filePath}"
+		resultId = result.get("check_id", "")
+		extras = result.get("extra", {})
+		line = result.get("start", {}).get("line", 0)
 		findings.append(
 			{
-				"id": result["check_id"],
-				"title": result["check_id"].split(".")[-1],
-				"description": result["extra"]["message"].strip(),
+				"id": resultId,
+				"title": resultId.split(".")[-1],
+				"description": extras("message").strip(),
 				"file": file,
-				"evidence": extractEvidence(result["start"]["line"], file),
-				"severity": levelMap[result["extra"]["severity"]],
+				"evidence": extractEvidence(line, file),
+				"severity": levelMap[extras("severity")],
 				"confidence": Level.HIGH,
-				"line": result["start"]["line"],
+				"line": line,
 				"_other": {
-					"col": result["start"]["col"],
-					"start": result["start"],
-					"end": result["end"],
-					"extra": result["extra"],
+					"end": result.get("end"),
+					"extra": extras,
 				},
 			}
 		)
 	return findings
```

### Comparing `simplesecurity-2023.0.1/simplesecurity/semgrep_sec.yaml` & `simplesecurity-2023.0.2/simplesecurity/semgrep_sec.yaml`

 * *Files identical despite different names*

### Comparing `simplesecurity-2023.0.1/simplesecurity/types.py` & `simplesecurity-2023.0.2/simplesecurity/types.py`

 * *Files identical despite different names*

### Comparing `simplesecurity-2023.0.1/setup.py` & `simplesecurity-2023.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
           'semgrep>=1.29.0,<2']}
 
 entry_points = \
 {'console_scripts': ['simplesecurity = simplesecurity:cli']}
 
 setup_kwargs = {
     'name': 'simplesecurity',
-    'version': '2023.0.1',
+    'version': '2023.0.2',
     'description': 'Combine multiple popular python security tools and generate reports or output into different formats',
     'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/simplesecurity.svg?style=for-the-badge)](https://pypistats.org/packages/simplesecurity)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsimplesecurity)](https://pepy.tech/project/simplesecurity)\n[![PyPI Version](https://img.shields.io/pypi/v/simplesecurity.svg?style=for-the-badge)](https://pypi.org/project/simplesecurity)\n\n<!-- omit in toc -->\n# SimpleSecurity\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nCombine multiple popular python security tools and generate reports or output\ninto different formats\n\nPlugins (these require the plugin executable in the system path. e.g. bandit\nrequires bandit to be in the system path...)\n\n- bandit\n- safety\n- dodgy\n- dlint\n- semgrep\n\nFormats\n\n- ansi (for terminal)\n- json\n- markdown\n- csv\n- sarif\n\n## Example Use\n\nSee below for the output if you run `simplesecurity` in this directory\n\n<img src="readme-assets/screenshots/sec.svg" width="500px">\n\n### Help\n\n```bash\n$ simplesecurity --help\nusage: simplesecurity [-h] [--scan-dir SCAN_DIR] [--format FORMAT] [--plugin PLUGIN] [--file FILE] [--level LEVEL]\n                      [--confidence CONFIDENCE] [--no-colour] [--high-contrast] [--fast] [--zero]\n\nCombine multiple popular python security tools and generate reports or output\ninto different formats...\n\noptions:\n  -h, --help            show this help message and exit\n  --scan-dir SCAN_DIR, -s SCAN_DIR\n                        Pass a path to the scan directory (optional)\n  --format FORMAT, -f FORMAT\n                        Output format. One of ansi, json, markdown, csv. default=ansi\n  --plugin PLUGIN, -p PLUGIN\n                        Plugin to use. One of bandit, safety, dodgy, dlint, semgrep, all, default=all\n  --file FILE, -o FILE  Filename to write to (omit for stdout)\n  --level LEVEL, -l LEVEL\n                        Minimum severity/ level to show\n  --confidence CONFIDENCE, -c CONFIDENCE\n                        Minimum confidence to show\n  --no-colour, -z       No ANSI colours\n  --high-contrast, -Z   High contrast colours\n  --fast, --skip        Skip long running jobs. Will omit plugins with long run time (applies to -p all only)\n  --zero, -0            Return non zero exit code if any security vulnerabilities are found\n```\n\nYou can also import this into your own project and use any of the functions\nin the DOCS\n\n<!-- omit in toc -->\n## Table of Contents\n\n- [Example Use](#example-use)\n\t- [Help](#help)\n- [Developer Notes](#developer-notes)\n\t- [Generate semgrep\\_sec.yaml](#generate-semgrep_secyaml)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Testing](#testing)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Developer Notes\n\n### Generate semgrep_sec.yaml\n\n1. Clone https://github.com/returntocorp/semgrep-rules\n2. cd to `semgrep-rules/python`\n3. do\n\n   ```bash\n   cat **/security/**/*.yaml >> semgrep_sec.yaml\n   cat **/security/*.yaml >> semgrep_sec.yaml\n   ```\n\n4. Find and replace `rules:` with `` apart from the first instance\n5. Reformat with `ctrl+shift+i`\n6. replace simplesecurity/semgrep_sec.yaml with the new one\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n**"Slim" Build:** Install bandit, dlint, dodgy, poetry, and safety with pipx\n\n```python\npip install simplesecurity\n```\n\n**Otherwise:**\n\n```python\npip install simplesecurity[full]\n```\n\nHead to https://pypi.org/project/SimpleSecurity/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Testing\n\nFor testing with the version of python used by poetry use\n\n```sh\npoetry run pytest\n```\n\nAlternatively use `tox` to run tests over python 3.8 - 3.11\n\n```sh\ntox\n```\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/SimpleSecurity\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
     'author': 'FredHappyface',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FHPythonUtils/SimpleSecurity',
```

### Comparing `simplesecurity-2023.0.1/PKG-INFO` & `simplesecurity-2023.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesecurity
-Version: 2023.0.1
+Version: 2023.0.2
 Summary: Combine multiple popular python security tools and generate reports or output into different formats
 Home-page: https://github.com/FHPythonUtils/SimpleSecurity
 License: MIT
 Author: FredHappyface
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

