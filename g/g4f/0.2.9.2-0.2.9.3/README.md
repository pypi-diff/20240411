# Comparing `tmp/g4f-0.2.9.2.tar.gz` & `tmp/g4f-0.2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.2.9.2.tar", last modified: Wed Apr 10 06:19:08 2024, max compression
+gzip compressed data, was "g4f-0.2.9.3.tar", last modified: Wed Apr 10 13:56:11 2024, max compression
```

## Comparing `g4f-0.2.9.2.tar` & `g4f-0.2.9.3.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.686904 g4f-0.2.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-10 06:19:04.000000 g4f-0.2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-10 06:19:04.000000 g4f-0.2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49099 2024-04-10 06:19:08.686904 g4f-0.2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45983 2024-04-10 06:19:04.000000 g4f-0.2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.650903 g4f-0.2.9.2/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.654903 g4f-0.2.9.2/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.658903 g4f-0.2.9.2/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.662903 g4f-0.2.9.2/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.662903 g4f-0.2.9.2/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.666903 g4f-0.2.9.2/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    31603 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.666903 g4f-0.2.9.2/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.666903 g4f-0.2.9.2/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.666903 g4f-0.2.9.2/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.666903 g4f-0.2.9.2/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.670903 g4f-0.2.9.2/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.670903 g4f-0.2.9.2/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.670903 g4f-0.2.9.2/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.670903 g4f-0.2.9.2/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.670903 g4f-0.2.9.2/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.674903 g4f-0.2.9.2/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.674903 g4f-0.2.9.2/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.674903 g4f-0.2.9.2/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.646903 g4f-0.2.9.2/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.674903 g4f-0.2.9.2/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22330 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.674903 g4f-0.2.9.2/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.674903 g4f-0.2.9.2/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    44113 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.678903 g4f-0.2.9.2/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.678903 g4f-0.2.9.2/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.678903 g4f-0.2.9.2/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.678903 g4f-0.2.9.2/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.682904 g4f-0.2.9.2/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.682904 g4f-0.2.9.2/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-10 06:19:04.000000 g4f-0.2.9.2/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:19:08.682904 g4f-0.2.9.2/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49099 2024-04-10 06:19:08.000000 g4f-0.2.9.2/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-10 06:19:08.000000 g4f-0.2.9.2/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:19:08.000000 g4f-0.2.9.2/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 06:19:08.000000 g4f-0.2.9.2/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-10 06:19:08.000000 g4f-0.2.9.2/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 06:19:08.000000 g4f-0.2.9.2/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:19:08.686904 g4f-0.2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-10 06:19:04.000000 g4f-0.2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.170579 g4f-0.2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-10 13:56:05.000000 g4f-0.2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-10 13:56:05.000000 g4f-0.2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49179 2024-04-10 13:56:11.170579 g4f-0.2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45983 2024-04-10 13:56:05.000000 g4f-0.2.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.130579 g4f-0.2.9.3/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.138579 g4f-0.2.9.3/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.138579 g4f-0.2.9.3/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.146579 g4f-0.2.9.3/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.146579 g4f-0.2.9.3/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.146579 g4f-0.2.9.3/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31603 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.150579 g4f-0.2.9.3/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.150579 g4f-0.2.9.3/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.150579 g4f-0.2.9.3/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.150579 g4f-0.2.9.3/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.150579 g4f-0.2.9.3/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.154579 g4f-0.2.9.3/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.154579 g4f-0.2.9.3/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.154579 g4f-0.2.9.3/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.154579 g4f-0.2.9.3/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.154579 g4f-0.2.9.3/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.158579 g4f-0.2.9.3/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.158579 g4f-0.2.9.3/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.126579 g4f-0.2.9.3/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.158579 g4f-0.2.9.3/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22551 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.158579 g4f-0.2.9.3/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.158579 g4f-0.2.9.3/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    45843 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.162579 g4f-0.2.9.3/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.162579 g4f-0.2.9.3/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.162579 g4f-0.2.9.3/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.162579 g4f-0.2.9.3/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.166579 g4f-0.2.9.3/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.166579 g4f-0.2.9.3/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-10 13:56:05.000000 g4f-0.2.9.3/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:56:11.166579 g4f-0.2.9.3/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49179 2024-04-10 13:56:11.000000 g4f-0.2.9.3/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-10 13:56:11.000000 g4f-0.2.9.3/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:56:11.000000 g4f-0.2.9.3/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 13:56:11.000000 g4f-0.2.9.3/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-10 13:56:11.000000 g4f-0.2.9.3/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 13:56:11.000000 g4f-0.2.9.3/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:56:11.170579 g4f-0.2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-10 13:56:05.000000 g4f-0.2.9.3/setup.py
```

### Comparing `g4f-0.2.9.2/LICENSE` & `g4f-0.2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/PKG-INFO` & `g4f-0.2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.2
+Version: 0.2.9.3
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -68,14 +68,16 @@
 Requires-Dist: flask; extra == "gui"
 Requires-Dist: beautifulsoup4; extra == "gui"
 Requires-Dist: pillow; extra == "gui"
 Requires-Dist: duckduckgo-search>=5.0; extra == "gui"
 Requires-Dist: browser_cookie3; extra == "gui"
 Provides-Extra: local
 Requires-Dist: gpt4all; extra == "local"
+Provides-Extra: curl-cffi
+Requires-Dist: curl_cffi>=0.6.2; extra == "curl-cffi"
 
 
 ![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
 
 <a href="https://trendshift.io/repositories/1692" target="_blank"><img src="https://trendshift.io/api/badge/repositories/1692" alt="xtekky%2Fgpt4free | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
 
 Written by [@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.2 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.3 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -34,19 +34,20 @@
 Extra: openai Requires-Dist: pycryptodome; extra == "openai" Provides-Extra:
 api Requires-Dist: loguru; extra == "api" Requires-Dist: fastapi; extra ==
 "api" Requires-Dist: uvicorn; extra == "api" Requires-Dist: nest_asyncio; extra
 == "api" Provides-Extra: gui Requires-Dist: werkzeug; extra == "gui" Requires-
 Dist: flask; extra == "gui" Requires-Dist: beautifulsoup4; extra == "gui"
 Requires-Dist: pillow; extra == "gui" Requires-Dist: duckduckgo-search>=5.0;
 extra == "gui" Requires-Dist: browser_cookie3; extra == "gui" Provides-Extra:
-local Requires-Dist: gpt4all; extra == "local" ![248433934-7886223b-c1d1-4260-
-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-
-76e0-496a-8ac4-e2de090cc6c9) _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|_ _T_r_e_n_d_s_h_i_f_t_]Written by
-[@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://
-github.com/hlohaus)
+local Requires-Dist: gpt4all; extra == "local" Provides-Extra: curl-cffi
+Requires-Dist: curl_cffi>=0.6.2; extra == "curl-cffi" ![248433934-7886223b-
+c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/
+98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9) _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|
+_T_r_e_n_d_s_h_i_f_t_]Written by [@xtekky](https://github.com/hlohaus) & maintained by
+[@hlohaus](https://github.com/hlohaus)
 > By using this repository or any code related to it, you agree to the [legal
 notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this
 repository nor endorses it**, nor is the author responsible for any copies,
 forks, re-uploads made by other users, or anything else related to GPT4Free.
 This is the author's only account and repository. To prevent impersonation or
 irresponsible actions, please comply with the GNU GPL license this Repository
 uses. > [!Warning] *"gpt4free"* serves as a **PoC** (proof of concept),
```

### Comparing `g4f-0.2.9.2/README.md` & `g4f-0.2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Aura.py` & `g4f-0.2.9.3/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Bing.py` & `g4f-0.2.9.3/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/BingCreateImages.py` & `g4f-0.2.9.3/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/ChatForAi.py` & `g4f-0.2.9.3/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Chatgpt4Online.py` & `g4f-0.2.9.3/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/ChatgptAi.py` & `g4f-0.2.9.3/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/ChatgptFree.py` & `g4f-0.2.9.3/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/ChatgptNext.py` & `g4f-0.2.9.3/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/ChatgptX.py` & `g4f-0.2.9.3/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/DeepInfra.py` & `g4f-0.2.9.3/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/DeepInfraImage.py` & `g4f-0.2.9.3/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/DuckDuckGo.py` & `g4f-0.2.9.3/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/FlowGpt.py` & `g4f-0.2.9.3/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/FreeChatgpt.py` & `g4f-0.2.9.3/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/FreeGpt.py` & `g4f-0.2.9.3/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/GeminiPro.py` & `g4f-0.2.9.3/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/GeminiProChat.py` & `g4f-0.2.9.3/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/GigaChat.py` & `g4f-0.2.9.3/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/GptTalkRu.py` & `g4f-0.2.9.3/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/HuggingChat.py` & `g4f-0.2.9.3/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/HuggingFace.py` & `g4f-0.2.9.3/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Koala.py` & `g4f-0.2.9.3/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Liaobots.py` & `g4f-0.2.9.3/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Llama2.py` & `g4f-0.2.9.3/g4f/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Local.py` & `g4f-0.2.9.3/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/PerplexityLabs.py` & `g4f-0.2.9.3/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Pi.py` & `g4f-0.2.9.3/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/Vercel.py` & `g4f-0.2.9.3/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.2.9.3/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/You.py` & `g4f-0.2.9.3/g4f/Provider/You.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import uuid
 
 from ..typing import AsyncResult, Messages, ImageType, Cookies
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .helper import format_prompt
 from ..image import ImageResponse, to_bytes, is_accepted_format
 from ..requests import StreamSession, FormData, raise_for_status
-from ..errors import MissingRequirementsError
-
 from .you.har_file import get_dfp_telemetry_id
 
 class You(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://you.com"
     working = True
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
```

### Comparing `g4f-0.2.9.2/g4f/Provider/__init__.py` & `g4f-0.2.9.3/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/bing/conversation.py` & `g4f-0.2.9.3/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/bing/create_images.py` & `g4f-0.2.9.3/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/bing/upload_image.py` & `g4f-0.2.9.3/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/AiService.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Aibn.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Aichat.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Ails.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Berlin.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Equing.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Forefront.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/H2o.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Myshell.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Phind.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/V50.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Vercel.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/deprecated/__init__.py` & `g4f-0.2.9.3/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.2.9.3/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/Groq.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/Openai.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/Poe.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/Theb.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.2.9.3/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/AItianhu.py` & `g4f-0.2.9.3/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/Bestim.py` & `g4f-0.2.9.3/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/ChatBase.py` & `g4f-0.2.9.3/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.2.9.3/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.2.9.3/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.2.9.3/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.2.9.3/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/Gpt6.py` & `g4f-0.2.9.3/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/GptChatly.py` & `g4f-0.2.9.3/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/GptForLove.py` & `g4f-0.2.9.3/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/GptGo.py` & `g4f-0.2.9.3/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/GptGod.py` & `g4f-0.2.9.3/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.2.9.3/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.2.9.3/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.2.9.3/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/npm/package-lock.json` & `g4f-0.2.9.3/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/openai/crypt.py` & `g4f-0.2.9.3/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/openai/har_file.py` & `g4f-0.2.9.3/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.2.9.3/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/selenium/Bard.py` & `g4f-0.2.9.3/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/selenium/MyShell.py` & `g4f-0.2.9.3/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.2.9.3/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/selenium/Phind.py` & `g4f-0.2.9.3/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/selenium/TalkAi.py` & `g4f-0.2.9.3/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.2.9.3/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.2.9.3/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/unfinished/Komo.py` & `g4f-0.2.9.3/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.2.9.3/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/Provider/you/har_file.py` & `g4f-0.2.9.3/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/__init__.py` & `g4f-0.2.9.3/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/api/__init__.py` & `g4f-0.2.9.3/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/api/_logging.py` & `g4f-0.2.9.3/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/cli.py` & `g4f-0.2.9.3/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/client/async_client.py` & `g4f-0.2.9.3/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/client/client.py` & `g4f-0.2.9.3/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/client/helper.py` & `g4f-0.2.9.3/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/client/image_models.py` & `g4f-0.2.9.3/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/client/service.py` & `g4f-0.2.9.3/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/client/stubs.py` & `g4f-0.2.9.3/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/client/types.py` & `g4f-0.2.9.3/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/cookies.py` & `g4f-0.2.9.3/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/errors.py` & `g4f-0.2.9.3/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/__init__.py` & `g4f-0.2.9.3/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/index.html` & `g4f-0.2.9.3/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/css/style.css` & `g4f-0.2.9.3/g4f/gui/client/static/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
     user-select: none;
     justify-content: space-between;
     border: 1px dashed var(--conversations);
     border-radius: var(--border-radius-1);
 }
 
 .conversations .convo .left {
+    width: 100%;
     cursor: pointer;
     display: flex;
     align-items: center;
     gap: 4px;
 }
 
 .conversations .convo .fa-ellipsis-vertical {
@@ -222,17 +223,19 @@
     color: var(--conversations);
     cursor: pointer;
 }
 
 .convo-title {
     color: var(--colour-3);
     font-size: 14px;
+    max-width: 100%;
     text-overflow: ellipsis;
     overflow: hidden; 
     white-space: nowrap;
+    margin-right: 10px;
 }
 
 .convo-title .datetime {
     font-size: 10px;
 }
 
 .message {
@@ -402,15 +405,15 @@
 
 .message .content .count {
     font-size: 12px;
 }
 
 .count_total {
     font-size: 12px;
-    padding-left: 100px;
+    padding-left: 25px;
     padding-top: 10px;
 }
 
 .new_convo {
     padding: 8px 12px;
     display: flex;
     gap: 18px;
@@ -642,27 +645,45 @@
     outline: none;
     padding: 8px 16px;
 
     appearance: none;
     width: 160px;
 }
 
+#systemPrompt, .settings textarea {
+    font-size: 15px;
+    width: 100%;
+    color: var(--colour-3);
+    min-height: 50px;
+    height: 59px;
+    outline: none;
+    padding: var(--inner-gap) var(--section-gap);
+    resize: vertical;
+}
+
+#systemPrompt {
+    padding-left: 35px;
+}
+
 @media only screen and (min-width: 40em) {
     select {
         width: 200px;
     }
     .field {
         padding-right: 15px
     }
     .message {
         flex-direction: row;
     }
     .settings .bottom_buttons {
         flex-direction: row;
     }
+    .count_total {
+        padding-left: 98px;
+    }
 }
 
 .input-box {
     display: flex;
     align-items: center;
     cursor: pointer;
 }
@@ -832,14 +853,18 @@
     .field {
         width: fit-content;
     }
 
     .mobile-sidebar {
         display: flex !important;
     }
+
+    #systemPrompt {
+        padding-left: 48px;
+    }
 }
 
 .shown {
     display: flex;
 }
 
 
@@ -1060,30 +1085,19 @@
     right: 8px;
 }
 
 #send-button:hover {
     border: 1px solid #e4d4ffc9;
 }
 
-#systemPrompt, .settings textarea {
-    font-size: 15px;
-    width: 100%;
-    color: var(--colour-3);
-    min-height: 50px;
-    height: 59px;
-    outline: none;
-    padding: var(--inner-gap) var(--section-gap);
-    resize: vertical;
-}
-
 .settings textarea {
     height: 51px;
 }
 
-.settings {
+.settings, .images {
     width: 100%;
     display: flex;
     flex-direction: column;
 }
 
 .settings .paper {
     overflow: auto;
```

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.2.9.3/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.2.9.3/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.2.9.3/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.2.9.3/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/img/gpt.png` & `g4f-0.2.9.3/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/img/user.png` & `g4f-0.2.9.3/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.2.9.3/g4f/gui/client/static/js/chat.v1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,21 +6,22 @@
 const regenerate = document.querySelector(`.regenerate`);
 const sidebar = document.querySelector(".conversations");
 const sidebar_button = document.querySelector(".mobile-sidebar");
 const sendButton = document.getElementById("send-button");
 const imageInput = document.getElementById("image");
 const cameraInput = document.getElementById("camera");
 const fileInput = document.getElementById("file");
-const microLabel = document.querySelector(".micro-label")
-const inputCount = document.getElementById("input-count")
+const microLabel = document.querySelector(".micro-label");
+const inputCount = document.getElementById("input-count");
 const providerSelect = document.getElementById("provider");
 const modelSelect = document.getElementById("model");
 const modelProvider = document.getElementById("model2");
-const systemPrompt = document.getElementById("systemPrompt")
-const settings = document.querySelector(".settings")
+const systemPrompt = document.getElementById("systemPrompt");
+const settings = document.querySelector(".settings");
+const album = document.querySelector(".images");
 
 let prompt_lock = false;
 
 let content, content_inner, content_count = null;
 
 const optionElements = document.querySelectorAll(".settings input, .settings textarea, #model, #model2, #provider")
 
@@ -45,30 +46,37 @@
             .replaceAll(/<!-- generated images start -->|<!-- generated images end -->/gm, "")
             .replaceAll(/<img data-prompt="[^>]+">/gm, "")
         )
         .replaceAll("<a href=", '<a target="_blank" href=')
         .replaceAll('<code>', '<code class="language-plaintext">')
 }
 
+function filter_message(text) {
+    return text.replaceAll(
+        /<!-- generated images start -->[\s\S]+<!-- generated images end -->/gm, ""
+    )
+}
+
 hljs.addPlugin(new CopyButtonPlugin());
 let typesetPromise = Promise.resolve();
 const highlight = (container) => {
     container.querySelectorAll('code:not(.hljs').forEach((el) => {
         if (el.className != "hljs") {
             hljs.highlightElement(el);
         }
     });
-    typesetPromise = typesetPromise.then(
-        () => MathJax.typesetPromise([container])
-    ).catch(
-        (err) => console.log('Typeset failed: ' + err.message)
-    );
+    if (window.MathJax) {
+        typesetPromise = typesetPromise.then(
+            () => MathJax.typesetPromise([container])
+        ).catch(
+            (err) => console.log('Typeset failed: ' + err.message)
+        );
+    }
 }
 
-let stopped = false;
 const register_message_buttons = async () => {
     document.querySelectorAll(".message .fa-xmark").forEach(async (el) => {
         if (!("click" in el.dataset)) {
             el.dataset.click = "true";
             el.addEventListener("click", async () => {
                 if (prompt_lock) {
                     return;
@@ -91,77 +99,85 @@
             })
         }
     });
     document.querySelectorAll(".message .fa-volume-high").forEach(async (el) => {
         if (!("click" in el.dataset)) {
             el.dataset.click = "true";
             el.addEventListener("click", async () => {
-                if ("active" in el.classList || window.doSpeech) {
-                    el.classList.add("blink")
-                    stopped = true;
-                    return;
+                let playlist = [];
+
+                function play_next() {
+                    const next = playlist.shift();
+                    if (next)
+                        next.play();
                 }
-                if (stopped) {
+                if (el.dataset.stopped) {
                     el.classList.remove("blink")
-                    stopped = false;
+                    delete el.dataset.stopped;
+                    return;
+                }
+                if (el.dataset.running) {
+                    el.dataset.stopped = true;
+                    el.classList.add("blink")
+                    playlist = [];
                     return;
                 }
+                el.dataset.running = true;
                 el.classList.add("blink")
                 el.classList.add("active")
-                const message_el = el.parentElement.parentElement.parentElement;
                 const content_el = el.parentElement.parentElement;
+                const message_el = content_el.parentElement;
                 let speechText = await get_message(window.conversation_id, message_el.dataset.index);
 
+                speechText = speechText.replaceAll(/([^0-9])\./gm, "$1.;");
+                speechText = speechText.replaceAll("?", "?;");
                 speechText = speechText.replaceAll(/\[(.+)\]\(.+\)/gm, "($1)");
-                speechText = speechText.replaceAll("`", "").replaceAll("#", "")
-                speechText = speechText.replaceAll(
-                    /<!-- generated images start -->[\s\S]+<!-- generated images end -->/gm,
-                    ""
-                )
+                speechText = speechText.replaceAll(/```[a-z]+/gm, "");
+                speechText = filter_message(speechText.replaceAll("`", "").replaceAll("#", ""))
+                const lines = speechText.trim().split(/\n|;/).filter(v => v.trim());
 
-                const lines = speechText.trim().split(/\n|\.|;/);
-                let ended = true;
                 window.onSpeechResponse = (url) => {
-                    el.classList.remove("blink")
+                    if (!el.dataset.stopped) {
+                        el.classList.remove("blink")
+                    }
                     if (url) {
                         var sound = document.createElement('audio');
                         sound.controls = 'controls';
                         sound.src = url;
                         sound.type = 'audio/wav';
                         sound.onended = function() {
-                            ended = true;
+                            el.dataset.do_play = true;
+                            setTimeout(play_next, 1000);
                         };
                         sound.onplay = function() {
-                            ended = false;
+                            delete el.dataset.do_play;
                         };
                         var container = document.createElement('div');
                         container.classList.add("audio");
                         container.appendChild(sound);
                         content_el.appendChild(container);
-                        if (ended && !stopped) {
-                            sound.play();
+                        if (!el.dataset.stopped) {
+                            playlist.push(sound);
+                            if (el.dataset.do_play) {
+                                play_next();
+                            }
                         }
                     }
-                    if (lines.length < 1 || stopped) {
+                    let line = lines.length > 0 ? lines.shift() : null;
+                    if (line && !el.dataset.stopped) {
+                        handleGenerateSpeech(line);
+                    } else {
                         el.classList.remove("active");
-                        return;
-                    }
-                    while (lines.length > 0) {
-                        let line = lines.shift();
-                        var reg = new RegExp('^[0-9]$');
-                        if (line && !reg.test(line)) {
-                            return handleGenerateSpeech(line);
-                        }
-                    }
-                    if (!line) {
-                        el.classList.remove("active")
+                        el.classList.remove("blink");
+                        delete el.dataset.running;
                     }
                 }
+                el.dataset.do_play = true;
                 let line = lines.shift();
-                return handleGenerateSpeech(line);
+                handleGenerateSpeech(line);
             });
         }
     });
 }
 
 const delete_conversations = async () => {
     for (let i = 0; i < appStorage.length; i++) {
@@ -398,15 +414,15 @@
         const file = input && input.files.length > 0 ? input.files[0] : null;
         const provider = providerSelect.options[providerSelect.selectedIndex].value;
         const auto_continue = document.getElementById("auto_continue")?.checked;
         if (file && !provider)
             provider = "Bing";
         let api_key = null;
         if (provider)
-            api_key = document.getElementById(`${provider}-api_key`)?.value;
+            api_key = document.getElementById(`${provider}-api_key`)?.value || null;
         await api("conversation", {
             id: window.token,
             conversation_id: window.conversation_id,
             model: get_selected_model(),
             web_search: document.getElementById("switch").checked,
             provider: provider,
             messages: messages,
@@ -563,20 +579,22 @@
                         <i class="fa-regular fa-clipboard"></i>
                     </div>
                 </div>
             </div>
         `;
     }
 
-    const filtered = prepare_messages(messages, false);
-    if (filtered.length > 0) {
-        last_model = last_model?.startsWith("gpt-4") ? "gpt-4" : "gpt-3.5-turbo"
-        let count_total = GPTTokenizer_cl100k_base?.encodeChat(filtered, last_model).length
-        if (count_total > 0) {
-            elements += `<div class="count_total">(${count_total} tokens used)</div>`;
+    if (window.GPTTokenizer_cl100k_base) {
+        const filtered = prepare_messages(messages, false);
+        if (filtered.length > 0) {
+            last_model = last_model?.startsWith("gpt-4") ? "gpt-4" : "gpt-3.5-turbo"
+            let count_total = GPTTokenizer_cl100k_base?.encodeChat(filtered, last_model).length
+            if (count_total > 0) {
+                elements += `<div class="count_total">(${count_total} tokens used)</div>`;
+            }
         }
     }
 
     message_box.innerHTML = elements;
     register_message_buttons();
     highlight(message_box);
     regenerate.classList.remove("regenerate-hidden");
@@ -605,28 +623,23 @@
     appStorage.setItem(
         `conversation:${conversation_id}`,
         JSON.stringify(conversation)
     );
 }
 
 async function get_messages(conversation_id) {
-    let conversation = await get_conversation(conversation_id);
+    const conversation = await get_conversation(conversation_id);
     return conversation?.items || [];
 }
 
 async function add_conversation(conversation_id, content) {
-    if (content.length > 18) {
-        title = content.substring(0, 18) + '...'
-    } else {
-        title = content + '&nbsp;'.repeat(20 - content.length)
-    }
     if (appStorage.getItem(`conversation:${conversation_id}`) == null) {
         await save_conversation(conversation_id, {
             id: conversation_id,
-            title: title,
+            title: "",
             added: Date.now(),
             system: systemPrompt?.value,
             items: [],
         });
     }
     history.pushState({}, null, `/chat/${conversation_id}`);
 }
@@ -692,21 +705,33 @@
     let conversations = [];
     for (let i = 0; i < appStorage.length; i++) {
         if (appStorage.key(i).startsWith("conversation:")) {
             let conversation = appStorage.getItem(appStorage.key(i));
             conversations.push(JSON.parse(conversation));
         }
     }
+    conversations.sort((a, b) => (b.updated || 0) - (a.updated || 0));
 
     await clear_conversations();
 
-    conversations.sort((a, b) => (b.updated || 0) - (a.updated || 0));
-
     let html = "";
     conversations.forEach((conversation) => {
+        if (conversation?.items.length > 0) {
+            let old_value = conversation.title;
+            let new_value = (conversation.items[0]["content"]).trim();
+            let new_lenght = new_value.indexOf("\n");
+            new_lenght = new_lenght > 200 || new_lenght < 0 ? 200 : new_lenght;
+            conversation.title = new_value.substring(0, new_lenght);
+            if (conversation.title != old_value) {
+                appStorage.setItem(
+                    `conversation:${conversation.id}`,
+                    JSON.stringify(conversation)
+                );
+            }
+        }
         let updated = "";
         if (conversation.updated) {
             const date = new Date(conversation.updated);
             updated = date.toLocaleString('en-GB', {
                 dateStyle: 'short',
                 timeStyle: 'short',
                 monthStyle: 'short'
@@ -723,15 +748,15 @@
                 <div id="cho-${conversation.id}" class="choise" style="display:none;">
                     <i onclick="delete_conversation('${conversation.id}')" class="fa-regular fa-trash"></i>
                     <i onclick="hide_option('${conversation.id}')" class="fa-regular fa-x"></i>
                 </div>
             </div>
         `;
     });
-    box_conversations.innerHTML = html;
+    box_conversations.innerHTML += html;
 };
 
 document.getElementById("cancelButton").addEventListener("click", async () => {
     window.controller.abort();
     if (!window.abort) {
         window.abort = true;
         content_inner.innerHTML += " [aborted]";
@@ -796,14 +821,25 @@
         settings.classList.remove("hidden");
         history.pushState({}, null, "/settings/");
     } else {
         settings.classList.add("hidden");
     }
 }
 
+function open_album() {
+    if (album.classList.contains("hidden")) {
+        sidebar.classList.remove("shown");
+        settings.classList.add("hidden");
+        album.classList.remove("hidden");
+        history.pushState({}, null, "/images/");
+    } else {
+        album.classList.add("hidden");
+    }
+}
+
 const register_settings_storage = async () => {
     optionElements.forEach((element) => {
         if (element.type == "textarea") {
             element.addEventListener('input', async (event) => {
                 appStorage.setItem(element.id, element.value);
             });
         } else {
@@ -897,22 +933,26 @@
         // fallback for no :has() support
         document.documentElement.className = themeOption.id;
     });
 });
 
 function count_tokens(model, text) {
     if (model) {
-        if (model.startsWith("llama2") || model.startsWith("codellama")) {
-            return llamaTokenizer?.encode(text).length;
-        }
-        if (model.startsWith("mistral") || model.startsWith("mixtral")) {
-            return mistralTokenizer?.encode(text).length;
-        }
+        if (window.llamaTokenizer)
+            if (model.startsWith("llama2") || model.startsWith("codellama")) {
+                return llamaTokenizer.encode(text).length;
+            }
+        if (window.mistralTokenizer)
+            if (model.startsWith("mistral") || model.startsWith("mixtral")) {
+                return mistralTokenizer.encode(text).length;
+            }
+    }
+    if (window.GPTTokenizer_cl100k_base) {
+        return GPTTokenizer_cl100k_base.encode(text).length;
     }
-    return GPTTokenizer_cl100k_base?.encode(text).length;
 }
 
 function count_words(text) {
     return text.trim().match(/[\w\u4E00-\u9FA5]+/gu)?.length || 0;
 }
 
 function count_chars(text) {
@@ -1247,46 +1287,51 @@
     function may_stop() {
         if (microLabel.classList.contains("recognition")) {
             recognition.stop();
         }
     }
 
     let startValue;
-    let lastValue;
     let timeoutHandle;
+    let lastDebounceTranscript;
     recognition.onstart = function() {
         microLabel.classList.add("recognition");
         startValue = messageInput.value;
-        lastValue = "";
+        lastDebounceTranscript = "";
         timeoutHandle = window.setTimeout(may_stop, 8000);
     };
     recognition.onend = function() {
         microLabel.classList.remove("recognition");
     };
     recognition.onresult = function(event) {
         if (!event.results) {
             return;
         }
         window.clearTimeout(timeoutHandle);
-        let newText;
-        Array.from(event.results).forEach((result) => {
-            newText = result[0].transcript;
-            if (newText && newText != lastValue) {
-                messageInput.value = `${startValue ? startValue+"\n" : ""}${newText.trim()}`;
-                if (result.isFinal) {
-                    lastValue = newText;
-                    startValue = messageInput.value;
-                    messageInput.focus();
-                }
-                messageInput.style.height = messageInput.scrollHeight + "px";
-                messageInput.scrollTop = messageInput.scrollHeight;
+
+        let result = event.results[event.resultIndex];
+        let isFinal = result.isFinal && (result[0].confidence > 0);
+        let transcript = result[0].transcript;
+        if (isFinal) {
+            if (transcript == lastDebounceTranscript) {
+                return;
             }
-        });
-        window.clearTimeout(timeoutHandle);
-        timeoutHandle = window.setTimeout(may_stop, newText ? 8000 : 5000);
+            lastDebounceTranscript = transcript;
+        }
+        if (transcript) {
+            messageInput.value = `${startValue ? startValue+"\n" : ""}${transcript.trim()}`;
+            if (isFinal) {
+                startValue = messageInput.value;
+                messageInput.focus();
+            }
+            messageInput.style.height = messageInput.scrollHeight + "px";
+            messageInput.scrollTop = messageInput.scrollHeight;
+        }
+
+        timeoutHandle = window.setTimeout(may_stop, transcript ? 8000 : 5000);
     };
 
     microLabel.addEventListener("click", () => {
         if (microLabel.classList.contains("recognition")) {
             window.clearTimeout(timeoutHandle);
             recognition.stop();
         } else {
```

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.2.9.3/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.2.9.3/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/js/icons.js` & `g4f-0.2.9.3/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.2.9.3/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.2.9.3/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.2.9.3/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/server/android_gallery.py` & `g4f-0.2.9.3/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/server/api.py` & `g4f-0.2.9.3/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/server/backend.py` & `g4f-0.2.9.3/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/server/config.py` & `g4f-0.2.9.3/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/server/internet.py` & `g4f-0.2.9.3/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/server/js_api.py` & `g4f-0.2.9.3/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/server/website.py` & `g4f-0.2.9.3/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/gui/webview.py` & `g4f-0.2.9.3/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/image.py` & `g4f-0.2.9.3/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/local/__init__.py` & `g4f-0.2.9.3/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/locals/models.py` & `g4f-0.2.9.3/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/locals/provider.py` & `g4f-0.2.9.3/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/models.py` & `g4f-0.2.9.3/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/providers/base_provider.py` & `g4f-0.2.9.3/g4f/providers/base_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             return "".join(cls.create_completion(model, messages, False, **kwargs))
 
         return await asyncio.wait_for(
             loop.run_in_executor(executor, create_func),
             timeout=kwargs.get("timeout")
         )
 
+    @classmethod
     def get_parameters(cls) -> dict:
         return signature(
             cls.create_async_generator if issubclass(cls, AsyncGeneratorProvider) else
             cls.create_async if issubclass(cls, AsyncProvider) else
             cls.create_completion
         ).parameters
 
@@ -103,15 +104,17 @@
 
         args = ""
         for name, param in cls.get_parameters().items():
             if name in ("self", "kwargs") or (name == "stream" and not cls.supports_stream):
                 continue
             args += f"\n    {name}"
             args += f": {get_type_name(param.annotation)}" if param.annotation is not Parameter.empty else ""
-            args += f' = "{param.default}"' if param.default == "" else f" = {param.default}" if param.default is not Parameter.empty else ""
+            default_value = f'"{param.default}"' if isinstance(param.default, str) else param.default
+            args += f" = {default_value}" if param.default is not Parameter.empty else ""
+            args += ","
         
         return f"g4f.Provider.{cls.__name__} supports: ({args}\n)"
 
 
 class AsyncProvider(AbstractProvider):
     """
     Provides asynchronous functionality for creating completions.
```

### Comparing `g4f-0.2.9.2/g4f/providers/create_images.py` & `g4f-0.2.9.3/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/providers/helper.py` & `g4f-0.2.9.3/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/providers/retry_provider.py` & `g4f-0.2.9.3/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/providers/types.py` & `g4f-0.2.9.3/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/requests/__init__.py` & `g4f-0.2.9.3/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/requests/aiohttp.py` & `g4f-0.2.9.3/g4f/requests/aiohttp.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,22 @@
         **kwargs
     ):
         if impersonate:
             headers = {
                 **DEFAULT_HEADERS,
                 **headers
             }
+        connect = None
+        if isinstance(timeout, tuple):
+            connect, timeout = timeout;
+        if timeout is not None:
+            timeout = ClientTimeout(timeout, connect)
         super().__init__(
             **kwargs,
-            timeout=ClientTimeout(timeout) if timeout else None,
+            timeout=timeout,
             response_class=StreamResponse,
             connector=get_connector(connector, proxies.get("all", proxies.get("https"))),
             headers=headers
         )
 
 def get_connector(connector: BaseConnector = None, proxy: str = None, rdns: bool = False) -> Optional[BaseConnector]:
     if proxy and not connector:
```

### Comparing `g4f-0.2.9.2/g4f/requests/curl_cffi.py` & `g4f-0.2.9.3/g4f/requests/curl_cffi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from __future__ import annotations
 
-from curl_cffi.requests import AsyncSession, Response, CurlMime
+from curl_cffi.requests import AsyncSession, Response
+try:
+    from curl_cffi.requests import CurlMime
+    has_curl_mime = True
+except ImportError:
+    has_curl_mime = False
 from typing import AsyncGenerator, Any
 from functools import partialmethod
 import json
 
 class StreamResponse:
     """
     A wrapper class for handling asynchronous streaming responses.
@@ -74,10 +79,15 @@
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
     post = partialmethod(request, "POST")
     put = partialmethod(request, "PUT")
     patch = partialmethod(request, "PATCH")
     delete = partialmethod(request, "DELETE")
 
-class FormData(CurlMime):
-    def add_field(self, name, data=None, content_type: str = None, filename: str = None) -> None:
-        self.addpart(name, content_type=content_type, filename=filename, data=data)
+if has_curl_mime:
+    class FormData(CurlMime):
+        def add_field(self, name, data=None, content_type: str = None, filename: str = None) -> None:
+            self.addpart(name, content_type=content_type, filename=filename, data=data)
+else:
+    class FormData():
+        def __init__(self) -> None:
+            raise RuntimeError("CurlMimi in curl_cffi is missing | pip install -U g4f[curl_cffi]")
```

### Comparing `g4f-0.2.9.2/g4f/requests/defaults.py` & `g4f-0.2.9.3/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/requests/raise_for_status.py` & `g4f-0.2.9.3/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/stubs.py` & `g4f-0.2.9.3/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/typing.py` & `g4f-0.2.9.3/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/version.py` & `g4f-0.2.9.3/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f/webdriver.py` & `g4f-0.2.9.3/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/g4f.egg-info/PKG-INFO` & `g4f-0.2.9.3/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.2
+Version: 0.2.9.3
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -68,14 +68,16 @@
 Requires-Dist: flask; extra == "gui"
 Requires-Dist: beautifulsoup4; extra == "gui"
 Requires-Dist: pillow; extra == "gui"
 Requires-Dist: duckduckgo-search>=5.0; extra == "gui"
 Requires-Dist: browser_cookie3; extra == "gui"
 Provides-Extra: local
 Requires-Dist: gpt4all; extra == "local"
+Provides-Extra: curl-cffi
+Requires-Dist: curl_cffi>=0.6.2; extra == "curl-cffi"
 
 
 ![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
 
 <a href="https://trendshift.io/repositories/1692" target="_blank"><img src="https://trendshift.io/api/badge/repositories/1692" alt="xtekky%2Fgpt4free | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
 
 Written by [@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.2 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.3 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -34,19 +34,20 @@
 Extra: openai Requires-Dist: pycryptodome; extra == "openai" Provides-Extra:
 api Requires-Dist: loguru; extra == "api" Requires-Dist: fastapi; extra ==
 "api" Requires-Dist: uvicorn; extra == "api" Requires-Dist: nest_asyncio; extra
 == "api" Provides-Extra: gui Requires-Dist: werkzeug; extra == "gui" Requires-
 Dist: flask; extra == "gui" Requires-Dist: beautifulsoup4; extra == "gui"
 Requires-Dist: pillow; extra == "gui" Requires-Dist: duckduckgo-search>=5.0;
 extra == "gui" Requires-Dist: browser_cookie3; extra == "gui" Provides-Extra:
-local Requires-Dist: gpt4all; extra == "local" ![248433934-7886223b-c1d1-4260-
-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-
-76e0-496a-8ac4-e2de090cc6c9) _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|_ _T_r_e_n_d_s_h_i_f_t_]Written by
-[@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://
-github.com/hlohaus)
+local Requires-Dist: gpt4all; extra == "local" Provides-Extra: curl-cffi
+Requires-Dist: curl_cffi>=0.6.2; extra == "curl-cffi" ![248433934-7886223b-
+c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/
+98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9) _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|
+_T_r_e_n_d_s_h_i_f_t_]Written by [@xtekky](https://github.com/hlohaus) & maintained by
+[@hlohaus](https://github.com/hlohaus)
 > By using this repository or any code related to it, you agree to the [legal
 notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this
 repository nor endorses it**, nor is the author responsible for any copies,
 forks, re-uploads made by other users, or anything else related to GPT4Free.
 This is the author's only account and repository. To prevent impersonation or
 irresponsible actions, please comply with the GNU GPL license this Repository
 uses. > [!Warning] *"gpt4free"* serves as a **PoC** (proof of concept),
```

### Comparing `g4f-0.2.9.2/g4f.egg-info/SOURCES.txt` & `g4f-0.2.9.3/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.2/setup.py` & `g4f-0.2.9.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         "werkzeug", "flask",
         "beautifulsoup4", "pillow",
         "duckduckgo-search>=5.0",
         "browser_cookie3"
     ],
     "local": [
         "gpt4all"
+    ],
+    "curl_cffi": [
+        "curl_cffi>=0.6.2",
     ]
 }
 
 DESCRIPTION = (
     'The official gpt4free repository | various collection of powerful language models'
 )
```

