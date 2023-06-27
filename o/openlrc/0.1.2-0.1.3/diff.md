# Comparing `tmp/openlrc-0.1.2.tar.gz` & `tmp/openlrc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-0.1.2.tar", max compression
+gzip compressed data, was "openlrc-0.1.3.tar", max compression
```

## Comparing `openlrc-0.1.2.tar` & `openlrc-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.2/LICENSE
--rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.2/openlrc/__init__.py
--rw-r--r--   0        0        0     6534 2023-06-22 22:44:31.210888 openlrc-0.1.2/openlrc/chatbot.py
--rw-r--r--   0        0        0      532 2023-06-09 19:56:29.876606 openlrc-0.1.2/openlrc/exceptions.py
--rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.2/openlrc/logger.py
--rw-r--r--   0        0        0     8777 2023-06-22 16:23:55.581748 openlrc-0.1.2/openlrc/openlrc.py
--rw-r--r--   0        0        0     5104 2023-06-20 09:23:36.095683 openlrc-0.1.2/openlrc/opt.py
--rw-r--r--   0        0        0     6782 2023-06-22 22:23:54.135290 openlrc-0.1.2/openlrc/prompter.py
--rw-r--r--   0        0        0     3071 2023-06-21 09:39:23.768067 openlrc-0.1.2/openlrc/subtitle.py
--rw-r--r--   0        0        0     5688 2023-06-21 02:12:44.479638 openlrc-0.1.2/openlrc/transcribe.py
--rw-r--r--   0        0        0     5592 2023-06-22 20:09:21.182541 openlrc-0.1.2/openlrc/translate.py
--rw-r--r--   0        0        0     3201 2023-06-20 08:37:49.043106 openlrc-0.1.2/openlrc/utils.py
--rw-r--r--   0        0        0     1158 2023-06-22 22:51:49.212478 openlrc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2436 2023-06-22 22:53:57.118364 openlrc-0.1.2/README.md
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 openlrc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.3/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.3/openlrc/__init__.py
+-rw-r--r--   0        0        0     6642 2023-06-24 22:32:18.752179 openlrc-0.1.3/openlrc/chatbot.py
+-rw-r--r--   0        0        0     2273 2023-06-26 16:59:34.458995 openlrc-0.1.3/openlrc/context.py
+-rw-r--r--   0        0        0      701 2023-06-25 03:24:03.534882 openlrc-0.1.3/openlrc/exceptions.py
+-rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.3/openlrc/logger.py
+-rw-r--r--   0        0        0    11568 2023-06-27 02:37:19.204604 openlrc-0.1.3/openlrc/openlrc.py
+-rw-r--r--   0        0        0     5160 2023-06-27 03:39:14.631067 openlrc-0.1.3/openlrc/opt.py
+-rw-r--r--   0        0        0     7768 2023-06-26 19:29:42.139607 openlrc-0.1.3/openlrc/prompter.py
+-rw-r--r--   0        0        0     3608 2023-06-27 02:39:59.839257 openlrc-0.1.3/openlrc/subtitle.py
+-rw-r--r--   0        0        0     5905 2023-06-26 02:59:37.362684 openlrc-0.1.3/openlrc/transcribe.py
+-rw-r--r--   0        0        0     5788 2023-06-26 19:30:54.045688 openlrc-0.1.3/openlrc/translate.py
+-rw-r--r--   0        0        0     5744 2023-06-25 13:45:28.650508 openlrc-0.1.3/openlrc/utils.py
+-rw-r--r--   0        0        0     1305 2023-06-27 04:24:27.572507 openlrc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3909 2023-06-27 02:28:07.921266 openlrc-0.1.3/README.md
+-rw-r--r--   0        0        0     5271 1970-01-01 00:00:00.000000 openlrc-0.1.3/PKG-INFO
```

### Comparing `openlrc-0.1.2/LICENSE` & `openlrc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.2/openlrc/chatbot.py` & `openlrc-0.1.3/openlrc/chatbot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#  Copyright (C) 2023. Hao Zheng
+#  All rights reserved.
+
 import asyncio
 import os
 import time
 from typing import List, Union, Dict, Callable
 
 import openai
 from aiohttp import ClientSession
@@ -56,15 +59,15 @@
         prompt_price, completion_price = self.pricing[self.model]
 
         prompt_tokens = response.usage['prompt_tokens']
         completion_tokens = response.usage['completion_tokens']
 
         self.api_fees[-1] += (prompt_tokens * prompt_price + completion_tokens * completion_price) / 1000
 
-    async def _create_achat(self, messages: List[Dict], output_checker: Callable = lambda x: True):
+    async def _create_achat(self, messages: List[Dict], output_checker: Callable = lambda *args, **kw: True):
         logger.debug(f'Raw content: {messages}')
 
         response = None
         for i in range(self.retry):
             try:
                 response = openai.ChatCompletion.create(
                     model=self.model,
@@ -103,26 +106,27 @@
             raise ChatBotException('Failed to create a chat.')
 
         if not output_checker(messages, response.choices[0].message.content):
             raise ChatBotException('Failed to create a chat. Invalid response format.')
 
         return response
 
-    async def _amessage(self, messages_list: List[List[Dict]], output_checker: Callable = lambda x: True):
+    async def _amessage(self, messages_list: List[List[Dict]], output_checker: Callable = lambda *args, **kw: True):
         """
         Async send messages to the GPT chatbot.
         """
         async with openai.aiosession.get(ClientSession()):
             results = await asyncio.gather(
                 *(self._create_achat(message, output_checker=output_checker) for message in messages_list)
             )
 
             return results
 
-    def message(self, messages_list: Union[List[Dict], List[List[Dict]]], output_checker: Callable = lambda x: True):
+    def message(self, messages_list: Union[List[Dict], List[List[Dict]]],
+                output_checker: Callable = lambda *args, **kw: True):
         """
         Send chunked messages to the GPT chatbot.
         """
         assert messages_list, 'Empty message list.'
 
         if isinstance(messages_list[0], dict):  # convert messages List[Dict] to messages_list List[List[Dict]]
             messages_list = [messages_list]
```

### Comparing `openlrc-0.1.2/openlrc/logger.py` & `openlrc-0.1.3/openlrc/logger.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.2/openlrc/opt.py` & `openlrc-0.1.3/openlrc/opt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+#  Copyright (C) 2023. Hao Zheng
+#  All rights reserved.
+
 import re
 from typing import Union
 
-import opencc
+import zhconv
 
 from openlrc.logger import logger
 from openlrc.subtitle import Subtitle
 from openlrc.utils import extend_filename
 
 
 class SubtitleOptimizer:
@@ -33,15 +36,15 @@
 
         logger.debug(f'Merge same text: {len(self.subtitle.segments)} -> {len(new_elements)}')
 
         self.subtitle.segments = new_elements
 
     def merge_short(self, threshold=1.5):
         """
-        Merge the short text.
+        Merge the short duration subtitle.
         """
         new_elements = []
 
         merged_element = None
         for i, element, in enumerate(self.subtitle.segments):
             if i == 0 or element.duration >= threshold:
                 if merged_element:
@@ -64,15 +67,15 @@
             else:
                 if not merged_element:
                     merged_element = element
                 else:
                     merged_element.text += ' ' + element.text
                     merged_element.end = element.end
 
-        logger.debug(f'Merge short text: {len(self.subtitle.segments)} -> {len(new_elements)}')
+        logger.debug(f'Merge the short duration subtitle: {len(self.subtitle.segments)} -> {len(new_elements)}')
 
         self.subtitle.segments = new_elements
 
     def merge_repeat(self):
         """
         Merge the same pattern in one lyric.
         :return:
@@ -100,27 +103,26 @@
         logger.debug('Cut long text done.')
 
         self.subtitle.segments = new_elements
 
     def traditional2mandarin(self):
         new_elements = self.subtitle.segments
 
-        converter = opencc.OpenCC('t2s.json')
         for i, element in enumerate(new_elements):
-            new_elements[i].text = converter.convert(element.text)
+            new_elements[i].text = zhconv.convert(element.text, locale='zh-cn')
 
         logger.debug('Traditional Chinese to Mandarin done.')
 
         self.subtitle.segments = new_elements
 
     def remove_unk(self):
         new_elements = self.subtitle.segments
 
         for i, element in enumerate(new_elements):
-            new_elements[i].text = element.text.replace('<unk>', ' ')
+            new_elements[i].text = element.text.replace('<unk>', '')
 
         logger.debug('Remove <unk> done.')
 
         self.subtitle.segments = new_elements
 
     def remove_empty(self):
         self.subtitle.segments = [element for element in self.subtitle.segments if element.text]
```

### Comparing `openlrc-0.1.2/openlrc/prompter.py` & `openlrc-0.1.3/openlrc/prompter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+#  Copyright (C) 2023. Hao Zheng
+#  All rights reserved.
+
 import re
 
 from langcodes import Language
+from lingua import LanguageDetectorBuilder
 
 from openlrc.logger import logger
 
+# instruction prompt modified from https://github.com/machinewrapped/gpt-subtrans
 base_instruction = f'''You are a translator, your task is to accurately revise and translate subtitles into a target language.
 The input are transcribed from audio, so there may be errors in the transcription. Please correct any errors you find in the sentences first, based on their context. Then translate them to target language according to the revised sentences.
 The user will provide a chunk of lines, you should respond with an accurate, concise, and natural-sounding translation for the dialogue. 
-The user may provide additional context, such as a synopsis or title of the film, a summary of the current scene, or a list of character names. Use this information to improve the quality of your translation.
+The user may provide additional context, such as background, synopsis or title of the film, a summary of the current scene, or a list of character names. Use this information to improve the quality of your translation.
 Your response will be processed by an automated system, so it is imperative that you adhere to the required output format.
 
 Example input (Japanese to Chinese):
 
 #200
 Original>
 変わりゆく時代において、
@@ -68,15 +73,15 @@
 <summary>John and Sarah discuss their plan to locate a suspect, deducing that he is likely in the uptown area.</summary>
 Remember to end this tag with ``</summary>``.
 
 Use the available information to add a short synopsis of the current scene in a <scene/> tag, for example:
 <scene>John and Sarah are in their office analyzing data and planning their next steps. They deduce that the suspect is probably in the uptown area and decide to start their search there.</scene>
 Remember to end this tag with ``</scene>``.
 
-Use the target language when writing content for the ``summary/`` and ``scene/`` tags. 
+Use the target language when writing content for the <summary/> and <scene/> tags. 
 Ensure that the summary and scene are concise, containing less than 100 words.
 You need to update your summary and scene with the new information you have.
 Do not guess or improvise if the context is unclear, just summarise the dialogue.
 
 The translation should be in a lovely colloquial style and suitable for high-quality subtitles.
 
 #######################
@@ -98,75 +103,87 @@
         raise NotImplementedError()
 
     def check_format(self, messages, output_str):
         raise NotImplementedError()
 
 
 class BaseTranslatePrompter(TranslatePrompter):
-    def __init__(self, src_lang, target_lang, audio_type=None, title='', synopsis=''):
-        self.src_lang = Language.get(src_lang).display_name('en')
-        self.target_lang = Language.get(target_lang).display_name('en')
-        if target_lang == 'zh-cn':
-            self.target_lang = 'Mandarin Chinese'
+    def __init__(self, src_lang, target_lang, audio_type=None, title='', background='', synopsis=''):
+        self.src_lang = src_lang
+        self.target_lang = target_lang
+        self.src_lang_display = Language.get(src_lang).display_name('en')
+        self.target_lang_display = Language.get(target_lang).display_name('en')
+        self.lan_detector = LanguageDetectorBuilder.from_all_languages().build()
 
         self.audio_type = audio_type
         self.title = title
+        self.background = background
         self.synopsis = synopsis
         self.user_prompt = f'''
 {f"<title>{self.title}</title>" if self.title else ""}
+{f"<background>{self.background}</background>" if self.background else ""}
 {f"<synopsis>{self.synopsis}</synopsis>" if self.synopsis else ""}
 <context>
 <scene>{{scene}}</scene>
 <chunk> {{summaries_str}} </chunk>
 </context>
 <chunk_id> Scene 1 Chunk {{chunk_num}} <chunk_id>
 
-Please translate these subtitles for {self.audio_type}{f" named {self.title}" if self.title else ""} from {self.src_lang} to {self.target_lang}.\n
+Please translate these subtitles for {self.audio_type}{f" named {self.title}" if self.title else ""} from {self.src_lang_display} to {self.target_lang_display}.\n
 {{user_input}}
 
-<summary/>
-<scene/>
-'''
+<summary></summary>
+<scene></scene>'''
 
     @staticmethod
     def system():
         return base_instruction
 
     def user(self, chunk_num, user_input, summaries='', scene=''):
         summaries_str = '\n'.join(f'Chunk {i}: {summary}' for i, summary in enumerate(summaries, 1))
         return self.user_prompt.format(summaries_str=summaries_str, scene=scene,
                                        chunk_num=chunk_num, user_input=user_input).strip()
 
     @classmethod
     def format_texts(cls, texts):
+        """
+        Reconstruct list of text into desired format.
+        :param texts: List of (id, text).
+        """
         return '\n'.join([f'#{i}\nOriginal>\n{text}\nTranslation>\n' for i, text in texts])
 
     def check_format(self, messages, content):
         summary = re.search(r'<summary>(.*)</summary>', content)
         scene = re.search(r'<scene>(.*)</scene>', content)
-        original = re.findall(r'Original>\n(.*?)\nTranslation>', content, re.DOTALL)
+        original = re.findall(r'Original>\n(.*?)\nTranslation>', messages[1]['content'], re.DOTALL)
         translation = re.findall(r'Translation>\n*(.*?)(?:#\d+|<summary>|\n*$)', content, re.DOTALL)
 
         if not original or not translation:
             logger.warning(f'Fail to extract original or translation.')
             logger.debug(f'Content: {content}')
             return False
 
         if len(original) != len(translation):
             logger.warning(
                 f'Fail to ensure length consistent: original is {len(original)}, translation is {len(translation)}')
             logger.debug(f'original: {original}')
             logger.debug(f'translation: {original}')
             return False
 
+        # Ensure the translated langauge is in the target language
+        translated_lang = self.lan_detector.detect_language_of(' '.join(translation)).name.lower()
+        target_lang = Language.get(self.target_lang).language_name().lower()
+        if translated_lang != target_lang:
+            logger.warning(f'Translated language is {translated_lang}, not {target_lang}.')
+            return False
+
         # It's ok to keep going without summary and scene
         if not summary or not summary.group(1):
             logger.warning(f'Fail to extract summary.')
             logger.debug(f'output_str: {content}')
-
         if not scene or not scene.group(1):
             logger.warning(f'Fail to extract scene.')
             logger.debug(f'output_str: {content}')
 
         return True
```

### Comparing `openlrc-0.1.2/openlrc/subtitle.py` & `openlrc-0.1.3/openlrc/subtitle.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#  Copyright (C) 2023. Hao Zheng
+#  All rights reserved.
+
 import json
 import sys
 from dataclasses import dataclass
 from functools import partial
 from typing import List, Union
 
 from openlrc.logger import logger
@@ -42,24 +45,30 @@
         with open(filename, encoding='utf-8') as f:
             content = json.loads(f.read())
 
         self.lang = content['language']
         self.generator = content['generator']
         self.segments: List[Element] = [Element(**seg) for seg in content['segments']]
 
+    def __len__(self):
+        return len(self.segments)
+
     def get_texts(self):
         return [e.text for e in self.segments]
 
-    def set_texts(self, texts):
+    def set_texts(self, texts, lang=None):
         # Check length
         assert len(texts) == len(self.segments)
 
         for i, text in enumerate(texts):
             self.segments[i].text = text
 
+        if lang:
+            self.lang = lang
+
     def save(self, filename, update_name=False):
         results = {
             'language': self.lang,
             'generator': self.generator,
             'segments': [seg.to_json() for seg in self.segments]
         }
 
@@ -68,14 +77,20 @@
 
         if update_name:
             self.filename = filename
 
         return filename
 
     def to_lrc(self):
+        # If duration larger than 1 hour, use srt file instead
+        if self.segments[-1].end >= 3600:
+            logger.warning('Duration larger than 1 hour, use srt file instead')
+            self.to_srt()
+            return
+
         lrc_name = change_ext(self.filename, 'lrc')
         fmt = partial(format_timestamp, fmt='lrc')
         with open(lrc_name, 'w', encoding='utf-8') as f:
             print(f'LRC generated by https://github.com/zh-plus/Open-Lyrics, lang={self.lang}', file=f, flush=True)
             for i, segment in enumerate(self.segments):
                 print(
                     f'[{fmt(segment.start)}] {segment.text}',
@@ -87,13 +102,14 @@
 
         logger.info(f'File saved to {lrc_name}')
 
     def to_srt(self):
         srt_name = change_ext(self.filename, 'srt')
         fmt = partial(format_timestamp, fmt='srt')
         with open(srt_name, 'w', encoding='utf-8') as f:
+            print(f'LRC generated by https://github.com/zh-plus/Open-Lyrics, lang={self.lang}', file=f, flush=True)
             for i, segment in enumerate(self.segments, start=1):
                 print(f'{i}\n'
                       f'{fmt(segment.start)} --> {fmt(segment.end)}\n'
                       f'{segment.text}\n\n', file=f, flush=True)
 
         logger.info(f'File saved to {srt_name}')
```

### Comparing `openlrc-0.1.2/openlrc/transcribe.py` & `openlrc-0.1.3/openlrc/transcribe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+#  Copyright (C) 2023. Hao Zheng
+#  All rights reserved.
+
 import json
 import re
 from typing import NamedTuple
 
-import librosa
 import whisperx
 from punctuators.models import PunctCapSegModelONNX
 
 from openlrc.logger import logger
-from openlrc.utils import Timer, release_memory
+from openlrc.utils import Timer, release_memory, get_audio_duration
 
 
 class TranscriptionInfo(NamedTuple):
     language: str
     duration: float
 
 
@@ -39,37 +41,41 @@
 
         with open('test_aligned_result.json', 'w', encoding='utf-8') as f:
             json.dump(aligned_result, f, ensure_ascii=False, indent=4)
 
         with Timer('Sentence Alignment'):
             pcs_result = self.sentence_align(aligned_result)
 
-        info = TranscriptionInfo(language=result['language'], duration=librosa.get_duration(filename=audio_path))
+        info = TranscriptionInfo(language=result['language'], duration=get_audio_duration(audio_path))
 
         return pcs_result, info
 
     @staticmethod
     def sentence_align(transcribe_result):
         """
         Align the word-level whisper transcribe result to sentence-level.
 
         :return A dict with key 'sentences' and value a list of dict with key 'text', 'start_word', 'end_word'.
         """
-        pcs_model = PunctCapSegModelONNX.from_pretrained('pcs_47lang')
-        punctuations = '.,?？，。、・।؟;።፣፧'
+        pcs_model: PunctCapSegModelONNX = PunctCapSegModelONNX.from_pretrained(
+            "1-800-BAD-CODE/xlm-roberta_punctuation_fullstop_truecase"
+        )
+        punctuations = '.,?？，。、・।؟;።፣፧،'
 
-        sentences_list = pcs_model.infer([segment['text'] for segment in transcribe_result['segments']])
+        sentences_list = pcs_model.infer([segment['text'] for segment in transcribe_result['segments']], apply_sbd=True)
 
         pcs_result = {'sentences': []}
         for segment, sentences in zip(transcribe_result['segments'], sentences_list):
             last_end_idx = 0
             for sentence in sentences:
                 sentence = sentence.lower()
-                stc_split = re.split(f'[{punctuations}]|<unk>', sentence)
-                # TODO: Recover <unk> from segment['text']
+                if '<unk>' in sentence:
+                    logger.error(f'Unknown token in sentence: {sentence}')
+
+                stc_split = re.split(f'[{punctuations}]', sentence)
 
                 # Remove empty string
                 stc_split = [split for split in stc_split if split]
 
                 if not stc_split:
                     continue
```

### Comparing `openlrc-0.1.2/openlrc/translate.py` & `openlrc-0.1.3/openlrc/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#  Copyright (C) 2023. Hao Zheng
+#  All rights reserved.
+
 import json
 import os
 import re
 import uuid
 
 import requests
 
@@ -67,22 +70,23 @@
 
             return summary.strip(), scene.strip(), [t.strip() for t in translation]
 
         except Exception as e:
             logger.error(f'Failed to extract contents from response: {content}')
             raise e
 
-    def translate(self, texts, src_lang, target_lang, audio_type='Anime', title='', synopsis='',
+    def translate(self, texts, src_lang, target_lang, audio_type='Anime', title='', background='', synopsis='',
                   compare_path='test_intermediate.json'):
         prompter: BaseTranslatePrompter = prompter_map[self.prompter](
-            src_lang, target_lang, audio_type, title=title, synopsis=synopsis)
+            src_lang, target_lang, audio_type, title=title, background=background, synopsis=synopsis)
         translate_bot = GPTBot(fee_limit=self.fee_limit)
         translate_bot.update(temperature=0.7)
 
         chunks = self.make_chunks(texts, chunk_size=self.chunk_size)
+        logger.info(f'Translating {title}: {len(chunks)} chunks, {len(texts)} lines in total.')
 
         # Start chunk-by-chunk translation
         translations = []
         summaries = []
         summary, scene = '', ''
         for i, chunk in enumerate(chunks, start=1):
             user_input = prompter.format_texts(chunk)
```

### Comparing `openlrc-0.1.2/pyproject.toml` & `openlrc-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "openlrc"
-version = "0.1.2"
+version = "0.1.3"
 description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
 license = "MIT"
 authors = [
     "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/zh-plus/Open-Lyrics"
@@ -39,13 +39,21 @@
 faster-whisper = "^0.6.0"
 tiktoken = "^0.3.1"
 langcodes = "^3.3.0"
 language-data = "^1.1"
 rich = "^12.6.0"
 tqdm = "^4.65.0"
 audioread = "^3.0.0"
-opencc = "^1.1.1"
+zhconv = "^1.4.3"
 punctuators = "^0.0.5"
 colorlog = "^6.7.0"
+pytest = "^7.4.0"
+ffmpeg-python = "^0.2.0"
+lingua-language-detector = "^1.3.2"
+
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/zh-plus/Open-Lyrics/issues"
```

### Comparing `openlrc-0.1.2/PKG-INFO` & `openlrc-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,22 +16,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: audioread (>=3.0.0,<4.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: faster-whisper (>=0.6.0,<0.7.0)
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
+Requires-Dist: lingua-language-detector (>=1.3.2,<2.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
-Requires-Dist: opencc (>=1.1.1,<2.0.0)
 Requires-Dist: punctuators (>=0.0.5,<0.0.6)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: tiktoken (>=0.3.1,<0.4.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: zhconv (>=1.4.3,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
 Description-Content-Type: text/markdown
 
 # Open-Lyrics
 
 Open-Lyrics is a Python library that transcribes voice files using
 [faster-whisper](https://github.com/guillaumekln/faster-whisper), and translates/polishes the resulting text
@@ -40,21 +43,26 @@
 ## Installation
 
 1. Please install CUDA and cuDNN first according to https://opennmt.net/CTranslate2/installation.html to
    enable `faster-whisper`.
 
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
-3. Install [whisperx](https://github.com/m-bain/whisperX)
+3. Install [PyTorch](https://pytorch.org/get-started/locally/):
+    ```shell
+   pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
+   ```
+
+4. Install [whisperx](https://github.com/m-bain/whisperX)
 
     ```shell
     pip install git+https://github.com/m-bain/whisperx.git
     ```
 
-4. This project can be installed from PyPI:
+5. This project can be installed from PyPI:
 
     ```shell
     pip install openlrc
     ```
 
    or install directly from GitHub:
 
@@ -71,32 +79,65 @@
 
 # Single file
 lrcer.run('./data/test.mp3', target_lang='zh-cn')  # Generate translated ./data/test.lrc with default translate prompt.
 
 # Multiple files
 lrcer.run(['./data/test1.mp3', './data/test2.mp3'], target_lang='zh-cn')
 # Note we run the transcription sequentially, but run the translation concurrently for each file.
+
+# Path can contain video
+lrcer.run(['./data/test_audio.mp3', './data/test_video.mp4'], target_lang='zh-cn')
+
+# Use context.yaml to improve translation
+lrcer.run('./data/test.mp3', target_lang='zh-cn', context_path='./data/context.yaml')
+```
+
+### Context
+
+Utilize the available context to enhance the quality of your translation.
+Save them as `context.yaml` in the same directory as your audio file.
+
+```yaml
+background: "This is a multi-line background.
+This is a basic example."
+audio_type: Movie
+synopsis_map: {
+  movie_name1 (without extension): "This
+  is a multi-line synopsis for movie1.",
+  movie_name2 (without extension): "This
+  is a multi-line synopsis for movie2.",
+  movie_name3 (without extension): "This is a single-line synopsis for movie 3.",
+}
 ```
 
 ## Todo
 
 - [x] [Efficiency] Batched translate/polish for GPT request (enable contextual ability).
 - [x] [Efficiency] Concurrent support for GPT request.
 - [x] [Efficiency & Transcription Quality] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
 - [x] [Translation Quality] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
 - [x] [Usability] Automatically fix json encoder error using GPT.
 - [x] [Efficiency] Asynchronously perform transcription and translation for multiple audio inputs.
 - [x] [Quality] Improve batched translation/polish prompt according
   to [gpt-subtrans](https://github.com/machinewrapped/gpt-subtrans).
+- [x] [Usability] Input video support.
 - [ ] [Usability] Multiple output format support.
+- [ ] [Quality]
+  Use [multilingual language model](https://www.sbert.net/docs/pretrained_models.html#multi-lingual-models) to assess
+  translation quality.
+- [ ] [Quality] Speech enhancement for input audio.
 - [ ] [Efficiency] Add Azure OpenAI Service support.
 - [ ] [Usability] Add local LLM support.
+- [ ] [Usability] Multiple translate engine (Microsoft, DeepL, Google, etc.) support.
 - [ ] [Others] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 
 ## Credits
 
 - https://github.com/guillaumekln/faster-whisper
+- https://github.com/m-bain/whisperX
 - https://github.com/openai/openai-python
 - https://github.com/openai/whisper
+- https://github.com/machinewrapped/gpt-subtrans
+- https://github.com/MicrosoftTranslator/Text-Translation-API-V3-Python
```

