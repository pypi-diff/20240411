# Comparing `tmp/spiceai-0.1.8.tar.gz` & `tmp/spiceai-0.1.9.tar.gz`

## Comparing `spiceai-0.1.8.tar` & `spiceai-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 spiceai-0.1.8/tags
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spiceai-0.1.8/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.1.8/.ropeproject/globalnames
--rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.1.8/.ropeproject/history
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 spiceai-0.1.8/scripts/run.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/errors.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/models.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/providers.py
--rw-r--r--   0        0        0    17415 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/spice.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/spice_message.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/utils.py
--rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/wrapped_clients.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.1.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.1.8/LICENSE
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 spiceai-0.1.8/README.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 spiceai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 spiceai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 spiceai-0.1.9/tags
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spiceai-0.1.9/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.1.9/.ropeproject/globalnames
+-rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.1.9/.ropeproject/history
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 spiceai-0.1.9/scripts/run.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/errors.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/models.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/providers.py
+-rw-r--r--   0        0        0    18856 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/spice.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/spice_message.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/utils.py
+-rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/wrapped_clients.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 spiceai-0.1.9/README.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 spiceai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 spiceai-0.1.9/PKG-INFO
```

### Comparing `spiceai-0.1.8/tags` & `spiceai-0.1.9/tags`

 * *Files 19% similar despite different names*

```diff
@@ -40,115 +40,138 @@
 !_TAG_PROGRAM_VERSION	6.0.0	//
 !_TAG_ROLE_DESCRIPTION!Python!module	imported	/imported modules/
 !_TAG_ROLE_DESCRIPTION!Python!module	indirectlyImported	/module imported in alternative name/
 !_TAG_ROLE_DESCRIPTION!Python!module	namespace	/namespace from where classes\/variables\/functions are imported/
 !_TAG_ROLE_DESCRIPTION!Python!unknown	imported	/imported from the other module/
 !_TAG_ROLE_DESCRIPTION!Python!unknown	indirectlyImported	/classes\/variables\/functions\/modules imported in alternative name/
 ANTHROPIC	spice/providers.py	/^ANTHROPIC = Provider("anthropic", get_anthropic_client)$/;"	v
+API Keys	README.md	/^### API Keys$/;"	S	section:Spice""Install
 APIConnectionError	spice/errors.py	/^class APIConnectionError(SpiceError):$/;"	c
 AZURE	spice/providers.py	/^AZURE = Provider("azure", get_azure_client)$/;"	v
 AuthenticationError	spice/errors.py	/^class AuthenticationError(SpiceError):$/;"	c
-CLAUDE_3_HAIKU_20240307	spice/models.py	/^CLAUDE_3_HAIKU_20240307 = TextModel("claude-3-haiku-20240307", ANTHROPIC, 200000)$/;"	v
-CLAUDE_3_OPUS_20240229	spice/models.py	/^CLAUDE_3_OPUS_20240229 = TextModel("claude-3-opus-20240229", ANTHROPIC, 200000)$/;"	v
+CLAUDE_3_HAIKU_20240307	spice/models.py	/^CLAUDE_3_HAIKU_20240307 = TextModel($/;"	v
+CLAUDE_3_OPUS_20240229	spice/models.py	/^CLAUDE_3_OPUS_20240229 = TextModel($/;"	v
 EmbeddingModel	spice/models.py	/^class EmbeddingModel(Model):$/;"	c
-GPT_35_TURBO_0125	spice/models.py	/^GPT_35_TURBO_0125 = TextModel("gpt-3.5-turbo-0125", OPEN_AI, 16385)$/;"	v
-GPT_4_0125_PREVIEW	spice/models.py	/^GPT_4_0125_PREVIEW = TextModel("gpt-4-0125-preview", OPEN_AI, 128000)$/;"	v
-GPT_4_VISION_PREVIEW	spice/models.py	/^GPT_4_VISION_PREVIEW = VisionModel("gpt-4-vision-preview", OPEN_AI, 128000)$/;"	v
+Embeddings and Transcriptions	README.md	/^### Embeddings and Transcriptions$/;"	S	section:Spice""Usage Examples
+GPT_35_TURBO_0125	spice/models.py	/^GPT_35_TURBO_0125 = TextModel("gpt-3.5-turbo-0125", OPEN_AI, input_cost=50, output_cost=150, con/;"	v
+GPT_4_0125_PREVIEW	spice/models.py	/^GPT_4_0125_PREVIEW = TextModel("gpt-4-0125-preview", OPEN_AI, input_cost=1000, output_cost=3000,/;"	v
+GPT_4_1106_PREVIEW	spice/models.py	/^GPT_4_1106_PREVIEW = TextModel("gpt-4-1106-preview", OPEN_AI, input_cost=1000, output_cost=3000,/;"	v
+GPT_4_1106_VISION_PREVIEW	spice/models.py	/^GPT_4_1106_VISION_PREVIEW = VisionModel($/;"	v
+GPT_4_TURBO	spice/models.py	/^GPT_4_TURBO = TextModel("gpt-4-turbo", OPEN_AI, input_cost=1000, output_cost=3000, context_lengt/;"	v
+GPT_4_TURBO_2024_04_09	spice/models.py	/^GPT_4_TURBO_2024_04_09 = TextModel($/;"	v
+GPT_4_TURBO_PREVIEW	spice/models.py	/^GPT_4_TURBO_PREVIEW = TextModel($/;"	v
+GPT_4_VISION_PREVIEW	spice/models.py	/^GPT_4_VISION_PREVIEW = VisionModel($/;"	v
+Install	README.md	/^## Install$/;"	s	chapter:Spice
 InvalidModelError	spice/errors.py	/^class InvalidModelError(SpiceError):$/;"	c
 InvalidProviderError	spice/errors.py	/^class InvalidProviderError(SpiceError):$/;"	c
 Mixing Providers	README.md	/^### Mixing Providers$/;"	S	section:Spice""Usage Examples
 Model	spice/models.py	/^class Model:$/;"	c
 NoAPIKeyError	spice/errors.py	/^class NoAPIKeyError(SpiceError):$/;"	c
 OPEN_AI	spice/providers.py	/^OPEN_AI = Provider("open_ai", get_openai_client)$/;"	v
 Provider	spice/providers.py	/^class Provider:$/;"	c
-ResponseFormatType	spice/spice.py	/^ResponseFormatType = Dict[str, Literal["text", "json"]]$/;"	v
+ResponseFormat	spice/spice.py	/^ResponseFormat = Dict[str, Literal["text", "json_object"]]$/;"	v
 Spice	README.md	/^# Spice$/;"	c
 Spice	spice/spice.py	/^class Spice:$/;"	c
 SpiceCallArgs	spice/spice.py	/^class SpiceCallArgs:$/;"	c
 SpiceError	spice/errors.py	/^class SpiceError(Exception):$/;"	c
 SpiceMessage	spice/spice_message.py	/^SpiceMessage = ChatCompletionMessageParam$/;"	v
 SpiceResponse	spice/spice.py	/^class SpiceResponse:$/;"	c
 Streaming	README.md	/^### Streaming$/;"	S	section:Spice""Usage Examples
 StreamingSpiceResponse	spice/spice.py	/^class StreamingSpiceResponse:$/;"	c
-TEXT_EMBEDDING_3_LARGE	spice/models.py	/^TEXT_EMBEDDING_3_LARGE = EmbeddingModel("text-embedding-3-large", OPEN_AI)$/;"	v
-TEXT_EMBEDDING_3_SMALL	spice/models.py	/^TEXT_EMBEDDING_3_SMALL = EmbeddingModel("text-embedding-3-small", OPEN_AI)$/;"	v
-TEXT_EMBEDDING_ADA_002	spice/models.py	/^TEXT_EMBEDDING_ADA_002 = EmbeddingModel("text-embedding-ada-002", OPEN_AI)$/;"	v
+TEXT_EMBEDDING_3_LARGE	spice/models.py	/^TEXT_EMBEDDING_3_LARGE = EmbeddingModel("text-embedding-3-large", OPEN_AI, input_cost=13)$/;"	v
+TEXT_EMBEDDING_3_SMALL	spice/models.py	/^TEXT_EMBEDDING_3_SMALL = EmbeddingModel("text-embedding-3-small", OPEN_AI, input_cost=2)$/;"	v
+TEXT_EMBEDDING_ADA_002	spice/models.py	/^TEXT_EMBEDDING_ADA_002 = EmbeddingModel("text-embedding-ada-002", OPEN_AI, input_cost=10)$/;"	v
 TextModel	spice/models.py	/^class TextModel(Model):$/;"	c
 TranscriptionModel	spice/models.py	/^class TranscriptionModel(Model):$/;"	c
-UnknownModel	spice/models.py	/^class UnknownModel(Model):$/;"	c
+UnknownModel	spice/models.py	/^class UnknownModel(TextModel, EmbeddingModel, TranscriptionModel):$/;"	c
 Usage Examples	README.md	/^## Usage Examples$/;"	s	chapter:Spice
 Using unknown models	README.md	/^### Using unknown models$/;"	S	section:Spice""Usage Examples
 VisionModel	spice/models.py	/^class VisionModel(TextModel):$/;"	c
-WHISPER_1	spice/models.py	/^WHISPER_1 = TranscriptionModel("whisper-1", OPEN_AI)$/;"	v
+WHISPER_1	spice/models.py	/^WHISPER_1 = TranscriptionModel("whisper-1", OPEN_AI, input_cost=1)$/;"	v
 WrappedAnthropicClient	spice/wrapped_clients.py	/^class WrappedAnthropicClient(WrappedClient):$/;"	c
 WrappedAzureClient	spice/wrapped_clients.py	/^class WrappedAzureClient(WrappedOpenAIClient):$/;"	c
 WrappedClient	spice/wrapped_clients.py	/^class WrappedClient(ABC):$/;"	c
 WrappedOpenAIClient	spice/wrapped_clients.py	/^class WrappedOpenAIClient(WrappedClient):$/;"	c
+_FakeWrappedOpenAIClient	spice/wrapped_clients.py	/^    class _FakeWrappedOpenAIClient(WrappedOpenAIClient):$/;"	c	class:WrappedAnthropicClient
 __aiter__	spice/spice.py	/^    def __aiter__(self):$/;"	m	class:StreamingSpiceResponse
 __anext__	spice/spice.py	/^    async def __anext__(self):$/;"	m	class:StreamingSpiceResponse
 __init__	spice/spice.py	/^    def __init__($/;"	m	class:Spice
-__init__	spice/spice.py	/^    def __init__(self, call_args: SpiceCallArgs, client: WrappedClient, stream: AsyncIterator):$/;"	m	class:StreamingSpiceResponse
+__init__	spice/spice.py	/^    def __init__($/;"	m	class:StreamingSpiceResponse
+__init__	spice/wrapped_clients.py	/^        def __init__(self):$/;"	m	class:WrappedAnthropicClient._FakeWrappedOpenAIClient
 __init__	spice/wrapped_clients.py	/^    def __init__(self, key):$/;"	m	class:WrappedAnthropicClient
 __init__	spice/wrapped_clients.py	/^    def __init__(self, key, base_url=None):$/;"	m	class:WrappedOpenAIClient
 __init__	spice/wrapped_clients.py	/^    def __init__(self, key, endpoint):$/;"	m	class:WrappedAzureClient
 __post_init__	spice/models.py	/^    def __post_init__(self):$/;"	m	class:Model
 __post_init__	spice/providers.py	/^    def __post_init__(self):$/;"	m	class:Provider
+_anthropic_token_multiplier	spice/wrapped_clients.py	/^    _anthropic_token_multiplier = 1.25$/;"	v	class:WrappedAnthropicClient
+_fake_openai_client	spice/wrapped_clients.py	/^    _fake_openai_client = _FakeWrappedOpenAIClient()$/;"	v	class:WrappedAnthropicClient
 _fix_call_args	spice/spice.py	/^    def _fix_call_args($/;"	m	class:Spice
 _get_client	spice/spice.py	/^    def _get_client(self, model: Model, provider: Optional[Provider | str]) -> WrappedClient:$/;"	m	class:Spice	typeref:typename:WrappedClient
-_get_embedding_model	spice/spice.py	/^    def _get_embedding_model(self, model: Optional[Model | str]) -> EmbeddingModel | UnknownMode/;"	m	class:Spice	typeref:typename:EmbeddingModel|UnknownModel
-_get_text_model	spice/spice.py	/^    def _get_text_model(self, model: Optional[Model | str]) -> TextModel | UnknownModel:$/;"	m	class:Spice	typeref:typename:TextModel|UnknownModel
-_get_transcription_model	spice/spice.py	/^    def _get_transcription_model(self, model: Model | str) -> TranscriptionModel | UnknownModel:$/;"	m	class:Spice	typeref:typename:TranscriptionModel|UnknownModel
+_get_embedding_model	spice/spice.py	/^    def _get_embedding_model(self, model: Optional[Model | str]) -> EmbeddingModel:$/;"	m	class:Spice	typeref:typename:EmbeddingModel
+_get_encoding_for_model	spice/wrapped_clients.py	/^    def _get_encoding_for_model(self, model: Model | str) -> tiktoken.Encoding:$/;"	m	class:WrappedOpenAIClient	typeref:typename:tiktoken.Encoding
+_get_text_model	spice/spice.py	/^    def _get_text_model(self, model: Optional[Model | str]) -> TextModel:$/;"	m	class:Spice	typeref:typename:TextModel
+_get_transcription_model	spice/spice.py	/^    def _get_transcription_model(self, model: Model | str) -> TranscriptionModel:$/;"	m	class:Spice	typeref:typename:TranscriptionModel
 azure_example	scripts/run.py	/^async def azure_example():$/;"	f
 basic_example	scripts/run.py	/^async def basic_example():$/;"	f
 catch_and_convert_errors	spice/wrapped_clients.py	/^    def catch_and_convert_errors(self) -> ContextManager[None]: ...$/;"	m	class:WrappedClient	typeref:typename:ContextManager[None]
 catch_and_convert_errors	spice/wrapped_clients.py	/^    def catch_and_convert_errors(self):$/;"	m	class:WrappedAnthropicClient
 catch_and_convert_errors	spice/wrapped_clients.py	/^    def catch_and_convert_errors(self):$/;"	m	class:WrappedOpenAIClient
 characters_per_second	spice/spice.py	/^    def characters_per_second(self) -> float:$/;"	m	class:SpiceResponse	typeref:typename:float
 complete_response	spice/spice.py	/^    async def complete_response(self) -> SpiceResponse:$/;"	m	class:StreamingSpiceResponse	typeref:typename:SpiceResponse
-count_messages_tokens	spice/utils.py	/^def count_messages_tokens(messages: list[SpiceMessage], model: str):$/;"	f
-count_string_tokens	spice/utils.py	/^def count_string_tokens(message: str, model: str, full_message: bool) -> int:$/;"	f	typeref:typename:int
+context_length	spice/models.py	/^    context_length: Optional[int] = field(default=None)$/;"	v	class:TextModel	typeref:typename:Optional[int]
+cost_callback	spice/spice.py	/^        def cost_callback(cost):$/;"	f	member:Spice.stream_response	file:
+count_messages_tokens	spice/wrapped_clients.py	/^    def count_messages_tokens(self, messages: List[SpiceMessage], model: Model | str) -> int:$/;"	m	class:WrappedAnthropicClient	typeref:typename:int
+count_messages_tokens	spice/wrapped_clients.py	/^    def count_messages_tokens(self, messages: List[SpiceMessage], model: Model | str) -> int:$/;"	m	class:WrappedClient	typeref:typename:int
+count_messages_tokens	spice/wrapped_clients.py	/^    def count_messages_tokens(self, messages: List[SpiceMessage], model: Model | str) -> int:$/;"	m	class:WrappedOpenAIClient	typeref:typename:int
+count_string_tokens	spice/wrapped_clients.py	/^    def count_string_tokens(self, message: str, model: Model | str, full_message: bool) -> int:$/;"	m	class:WrappedAnthropicClient	typeref:typename:int
+count_string_tokens	spice/wrapped_clients.py	/^    def count_string_tokens(self, message: str, model: Model | str, full_message: bool) -> int:$/;"	m	class:WrappedClient	typeref:typename:int
+count_string_tokens	spice/wrapped_clients.py	/^    def count_string_tokens(self, message: str, model: Model | str, full_message: bool) -> int:$/;"	m	class:WrappedOpenAIClient	typeref:typename:int
 current_response	spice/spice.py	/^    def current_response(self) -> SpiceResponse:$/;"	m	class:StreamingSpiceResponse	typeref:typename:SpiceResponse
-extract_text	spice/wrapped_clients.py	/^    def extract_text(self, chat_completion) -> str: ...$/;"	m	class:WrappedClient	typeref:typename:str
-extract_text	spice/wrapped_clients.py	/^    def extract_text(self, chat_completion):$/;"	m	class:WrappedAnthropicClient
-extract_text	spice/wrapped_clients.py	/^    def extract_text(self, chat_completion):$/;"	m	class:WrappedOpenAIClient
-fuzzy_model_lookup	spice/utils.py	/^def fuzzy_model_lookup(model_hint):$/;"	f
+embeddings_and_transcription_example	scripts/run.py	/^async def embeddings_and_transcription_example():$/;"	f
+embeddings_request_cost	spice/utils.py	/^def embeddings_request_cost(model: EmbeddingModel, input_tokens: int) -> Optional[float]:$/;"	f	typeref:typename:Optional[float]
+extract_text_and_tokens	spice/wrapped_clients.py	/^    def extract_text_and_tokens(self, chat_completion) -> tuple[str, int, int]: ...$/;"	m	class:WrappedClient	typeref:typename:tuple[str,int,int]
+extract_text_and_tokens	spice/wrapped_clients.py	/^    def extract_text_and_tokens(self, chat_completion):$/;"	m	class:WrappedAnthropicClient
+extract_text_and_tokens	spice/wrapped_clients.py	/^    def extract_text_and_tokens(self, chat_completion):$/;"	m	class:WrappedOpenAIClient
 get_anthropic_client	spice/providers.py	/^def get_anthropic_client(cache=[]):$/;"	f
 get_azure_client	spice/providers.py	/^def get_azure_client(cache=[]):$/;"	f
 get_chat_completion_or_stream	spice/wrapped_clients.py	/^    async def get_chat_completion_or_stream($/;"	m	class:WrappedClient	typeref:typename:ChatCompletion|AsyncIterator[ChatCompletionChunk]|Message|AsyncIterator[MessageStreamEvent]
 get_chat_completion_or_stream	spice/wrapped_clients.py	/^    async def get_chat_completion_or_stream(self, call_args: SpiceCallArgs):$/;"	m	class:WrappedAnthropicClient
 get_chat_completion_or_stream	spice/wrapped_clients.py	/^    async def get_chat_completion_or_stream(self, call_args: SpiceCallArgs):$/;"	m	class:WrappedOpenAIClient
-get_embeddings	spice/spice.py	/^    async def get_embeddings($/;"	m	class:Spice	typeref:typename:List[List[float]]
-get_embeddings	spice/wrapped_clients.py	/^    async def get_embeddings(self, input_texts: List[str], model: str) -> List[List[float]]: ...$/;"	m	class:WrappedClient	typeref:typename:List[List[float]]
-get_embeddings	spice/wrapped_clients.py	/^    async def get_embeddings(self, input_texts: List[str], model: str) -> List[List[float]]:$/;"	m	class:WrappedAnthropicClient	typeref:typename:List[List[float]]
-get_embeddings	spice/wrapped_clients.py	/^    async def get_embeddings(self, input_texts: List[str], model: str) -> List[List[float]]:$/;"	m	class:WrappedOpenAIClient	typeref:typename:List[List[float]]
-get_embeddings_sync	spice/spice.py	/^    def get_embeddings_sync($/;"	m	class:Spice	typeref:typename:List[List[float]]
-get_embeddings_sync	spice/wrapped_clients.py	/^    def get_embeddings_sync(self, input_texts: List[str], model: str) -> List[List[float]]: ...$/;"	m	class:WrappedClient	typeref:typename:List[List[float]]
-get_embeddings_sync	spice/wrapped_clients.py	/^    def get_embeddings_sync(self, input_texts: List[str], model: str) -> List[List[float]]:$/;"	m	class:WrappedAnthropicClient	typeref:typename:List[List[float]]
-get_embeddings_sync	spice/wrapped_clients.py	/^    def get_embeddings_sync(self, input_texts: List[str], model: str) -> List[List[float]]:$/;"	m	class:WrappedOpenAIClient	typeref:typename:List[List[float]]
-get_encoding_for_model	spice/utils.py	/^def get_encoding_for_model(model: str) -> tiktoken.Encoding:$/;"	f	typeref:typename:tiktoken.Encoding
-get_input_and_output_tokens	spice/wrapped_clients.py	/^    def get_input_and_output_tokens(self, chat_completion) -> tuple[int, int]: ...$/;"	m	class:WrappedClient	typeref:typename:tuple[int,int]
-get_input_and_output_tokens	spice/wrapped_clients.py	/^    def get_input_and_output_tokens(self, chat_completion):$/;"	m	class:WrappedAnthropicClient
-get_input_and_output_tokens	spice/wrapped_clients.py	/^    def get_input_and_output_tokens(self, chat_completion):$/;"	m	class:WrappedOpenAIClient
+get_embeddings	spice/spice.py	/^    async def get_embeddings($/;"	m	class:Spice	typeref:typename:Sequence[Sequence[float]]
+get_embeddings	spice/wrapped_clients.py	/^    async def get_embeddings(self, input_texts: List[str], model: str) -> Sequence[Sequence[floa/;"	m	class:WrappedAnthropicClient	typeref:typename:Sequence[Sequence[float]]
+get_embeddings	spice/wrapped_clients.py	/^    async def get_embeddings(self, input_texts: List[str], model: str) -> Sequence[Sequence[floa/;"	m	class:WrappedClient	typeref:typename:Sequence[Sequence[float]]
+get_embeddings	spice/wrapped_clients.py	/^    async def get_embeddings(self, input_texts: List[str], model: str) -> Sequence[Sequence[floa/;"	m	class:WrappedOpenAIClient	typeref:typename:Sequence[Sequence[float]]
+get_embeddings_sync	spice/spice.py	/^    def get_embeddings_sync($/;"	m	class:Spice	typeref:typename:Sequence[Sequence[float]]
+get_embeddings_sync	spice/wrapped_clients.py	/^    def get_embeddings_sync(self, input_texts: List[str], model: str) -> Sequence[Sequence[float/;"	m	class:WrappedAnthropicClient	typeref:typename:Sequence[Sequence[float]]
+get_embeddings_sync	spice/wrapped_clients.py	/^    def get_embeddings_sync(self, input_texts: List[str], model: str) -> Sequence[Sequence[float/;"	m	class:WrappedClient	typeref:typename:Sequence[Sequence[float]]
+get_embeddings_sync	spice/wrapped_clients.py	/^    def get_embeddings_sync(self, input_texts: List[str], model: str) -> Sequence[Sequence[float/;"	m	class:WrappedOpenAIClient	typeref:typename:Sequence[Sequence[float]]
 get_model_from_name	spice/models.py	/^def get_model_from_name(model_name: str) -> Model:$/;"	f	typeref:typename:Model
 get_openai_client	spice/providers.py	/^def get_openai_client(cache=[]):$/;"	f
 get_provider_from_name	spice/providers.py	/^def get_provider_from_name(provider_name: str) -> Provider:$/;"	f	typeref:typename:Provider
 get_response	spice/spice.py	/^    async def get_response($/;"	m	class:Spice	typeref:typename:SpiceResponse
 get_transcription	spice/spice.py	/^    async def get_transcription($/;"	m	class:Spice	typeref:typename:str
-get_transcription	spice/wrapped_clients.py	/^    async def get_transcription(self, audio_path: Path, model: str) -> str: ...$/;"	m	class:WrappedClient	typeref:typename:str
-get_transcription	spice/wrapped_clients.py	/^    async def get_transcription(self, audio_path: Path, model: str) -> str:$/;"	m	class:WrappedAnthropicClient	typeref:typename:str
-get_transcription	spice/wrapped_clients.py	/^    async def get_transcription(self, audio_path: Path, model: str) -> str:$/;"	m	class:WrappedOpenAIClient	typeref:typename:str
+get_transcription	spice/wrapped_clients.py	/^    async def get_transcription(self, audio_path: Path, model: str) -> tuple[str, float]: ...$/;"	m	class:WrappedClient	typeref:typename:tuple[str,float]
+get_transcription	spice/wrapped_clients.py	/^    async def get_transcription(self, audio_path: Path, model: str) -> tuple[str, float]:$/;"	m	class:WrappedAnthropicClient	typeref:typename:tuple[str,float]
+get_transcription	spice/wrapped_clients.py	/^    async def get_transcription(self, audio_path: Path, model: str) -> tuple[str, float]:$/;"	m	class:WrappedOpenAIClient	typeref:typename:tuple[str,float]
+input_cost	spice/models.py	/^    input_cost: Optional[int] = field(default=None)$/;"	v	class:EmbeddingModel	typeref:typename:Optional[int]
+input_cost	spice/models.py	/^    input_cost: Optional[int] = field(default=None)$/;"	v	class:TextModel	typeref:typename:Optional[int]
+input_cost	spice/models.py	/^    input_cost: Optional[int] = field(default=None)$/;"	v	class:TranscriptionModel	typeref:typename:Optional[int]
 load_provider	spice/spice.py	/^    def load_provider(self, provider: Provider | str):$/;"	m	class:Spice
 max_tokens	spice/spice.py	/^    max_tokens: Optional[int] = None$/;"	v	class:SpiceCallArgs	typeref:typename:Optional[int]
 models	spice/models.py	/^models: List[Model] = []$/;"	v	typeref:typename:List[Model]
 multiple_providers_example	scripts/run.py	/^async def multiple_providers_example():$/;"	f
+output_cost	spice/models.py	/^    output_cost: Optional[int] = field(default=None)$/;"	v	class:TextModel	typeref:typename:Optional[int]
 process_chunk	spice/wrapped_clients.py	/^    def process_chunk(self, chunk) -> tuple[Optional[str], Optional[int], Optional[int]]: ...$/;"	m	class:WrappedClient	typeref:typename:tuple[Optional[str],Optional[int],Optional[int]]
 process_chunk	spice/wrapped_clients.py	/^    def process_chunk(self, chunk):$/;"	m	class:WrappedAnthropicClient
 process_chunk	spice/wrapped_clients.py	/^    def process_chunk(self, chunk):$/;"	m	class:WrappedOpenAIClient
 providers	spice/providers.py	/^providers: List[Provider] = []$/;"	v	typeref:typename:List[Provider]
-response_format	spice/spice.py	/^    response_format: Optional[ResponseFormatType] = None$/;"	v	class:SpiceCallArgs	typeref:typename:Optional[ResponseFormatType]
+response_format	spice/spice.py	/^    response_format: Optional[ResponseFormat] = None$/;"	v	class:SpiceCallArgs	typeref:typename:Optional[ResponseFormat]
 run_all_examples	scripts/run.py	/^async def run_all_examples():$/;"	f
 stream	spice/spice.py	/^    stream: bool = False$/;"	v	class:SpiceCallArgs	typeref:typename:bool
 stream_response	spice/spice.py	/^    async def stream_response($/;"	m	class:Spice	typeref:typename:StreamingSpiceResponse
 streaming_example	scripts/run.py	/^async def streaming_example():$/;"	f
 temperature	spice/spice.py	/^    temperature: Optional[float] = None$/;"	v	class:SpiceCallArgs	typeref:typename:Optional[float]
+text_request_cost	spice/utils.py	/^def text_request_cost(model: TextModel, input_tokens: int, output_tokens: int) -> Optional[float/;"	f	typeref:typename:Optional[float]
 timer	spice/spice.py	/^from timeit import default_timer as timer$/;"	Y	nameref:unknown:default_timer
+total_cost	spice/spice.py	/^    def total_cost(self) -> float:$/;"	m	class:Spice	typeref:typename:float
 total_tokens	spice/spice.py	/^    def total_tokens(self) -> int:$/;"	m	class:SpiceResponse	typeref:typename:int
+transcription_request_cost	spice/utils.py	/^def transcription_request_cost(model: TranscriptionModel, input_length: float) -> Optional[float/;"	f	typeref:typename:Optional[float]
```

### Comparing `spiceai-0.1.8/.github/workflows/ruff.yml` & `spiceai-0.1.9/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.8/.ropeproject/globalnames` & `spiceai-0.1.9/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.8/.ropeproject/history` & `spiceai-0.1.9/.ropeproject/history`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.8/spice/providers.py` & `spiceai-0.1.9/spice/providers.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.8/spice/spice.py` & `spiceai-0.1.9/spice/spice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
 from timeit import default_timer as timer
-from typing import AsyncIterator, Dict, List, Literal, Optional, cast
+from typing import AsyncIterator, Callable, Dict, List, Literal, Optional, Sequence, cast
 
 from spice.errors import InvalidModelError
-from spice.models import EmbeddingModel, Model, TextModel, TranscriptionModel, UnknownModel, get_model_from_name
+from spice.models import EmbeddingModel, Model, TextModel, TranscriptionModel, get_model_from_name
 from spice.providers import Provider, get_provider_from_name
 from spice.spice_message import SpiceMessage
-from spice.utils import count_messages_tokens, count_string_tokens
+from spice.utils import embeddings_request_cost, text_request_cost, transcription_request_cost
 from spice.wrapped_clients import WrappedClient
 
-ResponseFormatType = Dict[str, Literal["text", "json"]]
+ResponseFormat = Dict[str, Literal["text", "json_object"]]
 
 
 @dataclass
 class SpiceCallArgs:
     model: str
     messages: List[SpiceMessage]
     stream: bool = False
     temperature: Optional[float] = None
     max_tokens: Optional[int] = None
-    response_format: Optional[ResponseFormatType] = None
+    response_format: Optional[ResponseFormat] = None
 
 
 @dataclass
 class SpiceResponse:
     """
     Contains a collection of information about a completed LLM call.
     """
@@ -34,29 +34,27 @@
     call_args: SpiceCallArgs
     """The call arguments given to the model that created this response."""
 
     text: str
     """The total text sent by the model."""
 
     total_time: float
-    """
-    How long it took for the response to be completed.
-    May be inaccurate for streamed responses if not iterated over and completed immediately.
-    """
+    """How long it took for the response to be completed. May be inaccurate for incomplete streamed responses."""
 
     input_tokens: int
-    """The number of input tokens given in this response."""
+    """The number of input tokens given in this response. May be inaccurate for incomplete streamed responses."""
 
     output_tokens: int
-    """The number of output tokens given by the model in this response."""
+    """The number of output tokens given by the model in this response. May be inaccurate for incomplete streamed responses."""
 
     completed: bool
-    """Whether or not this response was fully completed. This will only ever be false for streaming responses."""
+    """Whether or not this response was fully completed. This will only ever be false for incomplete streamed responses."""
 
-    # TODO: Add cost
+    cost: Optional[float]
+    """The cost of this request in cents. May be inaccurate for incompleted streamed responses. Will be None if the cost of the model used is not known."""
 
     @property
     def total_tokens(self) -> int:
         """The total tokens, input and output, in this response."""
         return self.input_tokens + self.output_tokens
 
     @property
@@ -66,24 +64,34 @@
 
 
 class StreamingSpiceResponse:
     """
     Returned from a streaming llm call. Can be iterated over asynchronously to retrieve the content.
     """
 
-    def __init__(self, call_args: SpiceCallArgs, client: WrappedClient, stream: AsyncIterator):
+    def __init__(
+        self,
+        model: TextModel,
+        call_args: SpiceCallArgs,
+        client: WrappedClient,
+        stream: AsyncIterator,
+        cost_callback: Callable[[float], None],
+    ):
+        self._model = model
         self._call_args = call_args
         self._text = []
         self._start_time = timer()
         self._end_time = None
         self._input_tokens = None
         self._output_tokens = None
         self._finished = False
         self._client = client
         self._stream = stream
+        self._cost_added = 0
+        self._cost_callback = cost_callback
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
         with self._client.catch_and_convert_errors():
             try:
@@ -108,32 +116,35 @@
         Will not wait for the LLM call to finish.
         """
         if not self._finished or self._end_time is None:
             self._end_time = timer()
 
         full_output = "".join(self._text)
 
-        # TODO: this message counting methods are just for OpenAI,
-        # if other providers also don't send token counts when streaming or are interrupted
-        # then we need to add counting methods for them as well.
-        # Easiest way to do this would be to add count tokens functions to wrapped client
         input_tokens = self._input_tokens
         if input_tokens is None:
-            input_tokens = count_messages_tokens(self._call_args.messages, self._call_args.model)
+            input_tokens = self._client.count_messages_tokens(self._call_args.messages, self._model)
         output_tokens = self._output_tokens
         if output_tokens is None:
-            output_tokens = count_string_tokens(full_output, self._call_args.model, full_message=False)
+            output_tokens = self._client.count_string_tokens(full_output, self._model, full_message=False)
+
+        cost = text_request_cost(self._model, input_tokens, output_tokens)
+        if cost is not None:
+            new_cost = cost - self._cost_added
+            self._cost_added = cost
+            self._cost_callback(new_cost)
 
         return SpiceResponse(
             self._call_args,
             full_output,
             self._end_time - self._start_time,
             input_tokens,
             output_tokens,
             self._finished,
+            cost,
         )
 
     async def complete_response(self) -> SpiceResponse:
         """
         Waits until the entire LLM call finishes, collects it, and returns its SpiceResponse.
         """
         async for _ in self:
@@ -166,29 +177,36 @@
             model_aliases: A custom model name map.
         """
 
         if isinstance(default_text_model, str):
             text_model = get_model_from_name(default_text_model)
         else:
             text_model = default_text_model
-        if text_model and not isinstance(text_model, (TextModel, UnknownModel)):
+        if text_model and not isinstance(text_model, TextModel):
             raise InvalidModelError("Default text model must be a text model")
         self._default_text_model = text_model
 
         if isinstance(default_embeddings_model, str):
             embeddings_model = get_model_from_name(default_embeddings_model)
         else:
             embeddings_model = default_embeddings_model
-        if embeddings_model and not isinstance(embeddings_model, (EmbeddingModel, UnknownModel)):
+        if embeddings_model and not isinstance(embeddings_model, EmbeddingModel):
             raise InvalidModelError("Default embeddings model must be an embeddings model")
         self._default_embeddings_model = embeddings_model
 
         # TODO: Should we validate model aliases?
         self._model_aliases = model_aliases
 
+        self._total_cost: float = 0
+
+    @property
+    def total_cost(self) -> float:
+        """The total cost in cents of all api calls made through this Spice client."""
+        return self._total_cost
+
     def load_provider(self, provider: Provider | str):
         """
         Loads the specified provider and raises a NoAPIKeyError if no valid api key for the provider is found.
         Providers not preloaded will be loaded on first use, and the NoAPIKeyError will be raised when they are used.
         """
 
         if isinstance(provider, str):
@@ -201,39 +219,39 @@
                 provider = get_provider_from_name(provider)
             return provider.get_client()
         else:
             if model.provider is None:
                 raise InvalidModelError("Provider is required when unknown models are used")
             return model.provider.get_client()
 
-    def _get_text_model(self, model: Optional[Model | str]) -> TextModel | UnknownModel:
+    def _get_text_model(self, model: Optional[Model | str]) -> TextModel:
         if model is None:
             if self._default_text_model is None:
                 raise InvalidModelError("Model is required when default text model is not set at initialization")
             model = self._default_text_model
 
         if self._model_aliases is not None and model in self._model_aliases:
             model = self._model_aliases[model]
 
         if isinstance(model, str):
             model = get_model_from_name(model)
 
-        if not isinstance(model, (TextModel, UnknownModel)):
+        if not isinstance(model, TextModel):
             raise InvalidModelError(f"Model {model} is not a text model")
 
         return model
 
     def _fix_call_args(
         self,
         messages: List[SpiceMessage],
         model: Model,
         stream: bool,
         temperature: Optional[float],
         max_tokens: Optional[int],
-        response_format: Optional[ResponseFormatType],
+        response_format: Optional[ResponseFormat],
     ):
         # Not all providers support response format
         if response_format is not None:
             if response_format == {"type": "text"}:
                 response_format = None
 
         return SpiceCallArgs(
@@ -248,15 +266,15 @@
     async def get_response(
         self,
         messages: List[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
-        response_format: Optional[ResponseFormatType] = None,
+        response_format: Optional[ResponseFormat] = None,
     ) -> SpiceResponse:
         """
         Asynchronously retrieves a chat completion response.
 
         Args:
             messages: The list of messages given as context for the completion.
 
@@ -278,29 +296,31 @@
         client = self._get_client(text_model, provider)
         call_args = self._fix_call_args(messages, text_model, False, temperature, max_tokens, response_format)
 
         start_time = timer()
         with client.catch_and_convert_errors():
             chat_completion = await client.get_chat_completion_or_stream(call_args)
         end_time = timer()
-        input_tokens, output_tokens = client.get_input_and_output_tokens(chat_completion)
+        text, input_tokens, output_tokens = client.extract_text_and_tokens(chat_completion)
 
-        response = SpiceResponse(
-            call_args, client.extract_text(chat_completion), end_time - start_time, input_tokens, output_tokens, True
-        )
+        cost = text_request_cost(text_model, input_tokens, output_tokens)
+        if cost is not None:
+            self._total_cost += cost
+
+        response = SpiceResponse(call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost)
         return response
 
     async def stream_response(
         self,
         messages: List[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
-        response_format: Optional[ResponseFormatType] = None,
+        response_format: Optional[ResponseFormat] = None,
     ) -> StreamingSpiceResponse:
         """
         Asynchronously retrieves a chat completion stream that can be iterated over asynchronously.
 
         Args:
             messages: The list of messages given as context for the completion.
 
@@ -321,39 +341,43 @@
         text_model = self._get_text_model(model)
         client = self._get_client(text_model, provider)
         call_args = self._fix_call_args(messages, text_model, True, temperature, max_tokens, response_format)
 
         with client.catch_and_convert_errors():
             stream = await client.get_chat_completion_or_stream(call_args)
         stream = cast(AsyncIterator, stream)
-        return StreamingSpiceResponse(call_args, client, stream)
 
-    def _get_embedding_model(self, model: Optional[Model | str]) -> EmbeddingModel | UnknownModel:
+        def cost_callback(cost):
+            self._total_cost += cost
+
+        return StreamingSpiceResponse(text_model, call_args, client, stream, cost_callback)
+
+    def _get_embedding_model(self, model: Optional[Model | str]) -> EmbeddingModel:
         if model is None:
             if self._default_embeddings_model is None:
                 raise InvalidModelError("Model is required when default embeddings model is not set at initialization")
             model = self._default_embeddings_model
 
         if self._model_aliases is not None and model in self._model_aliases:
             model = self._model_aliases[model]
 
         if isinstance(model, str):
             model = get_model_from_name(model)
 
-        if not isinstance(model, (EmbeddingModel, UnknownModel)):
+        if not isinstance(model, EmbeddingModel):
             raise InvalidModelError(f"Model {model} is not a embedding model")
 
         return model
 
     async def get_embeddings(
         self,
         input_texts: List[str],
         model: Optional[EmbeddingModel | str] = None,
         provider: Optional[Provider | str] = None,
-    ) -> List[List[float]]:
+    ) -> Sequence[Sequence[float]]:
         """
         Asynchronously retrieves embeddings for a list of text.
 
         Args:
             input_texts: The texts to generate embeddings for.
 
             model: The embedding model to use. If no model is given, will use the default embedding model
@@ -362,22 +386,27 @@
 
             provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
         """
 
         embedding_model = self._get_embedding_model(model)
         client = self._get_client(embedding_model, provider)
 
+        input_tokens = sum(client.count_string_tokens(text, embedding_model, False) for text in input_texts)
+        cost = embeddings_request_cost(embedding_model, input_tokens)
+        if cost is not None:
+            self._total_cost += cost
+
         return await client.get_embeddings(input_texts, embedding_model.name)
 
     def get_embeddings_sync(
         self,
         input_texts: List[str],
         model: Optional[EmbeddingModel | str] = None,
         provider: Optional[Provider | str] = None,
-    ) -> List[List[float]]:
+    ) -> Sequence[Sequence[float]]:
         """
         Synchronously retrieves embeddings for a list of text.
 
         Args:
             input_texts: The texts to generate embeddings for.
 
             model: The embedding model to use. If no model is given, will use the default embedding model
@@ -386,31 +415,36 @@
 
             provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
         """
 
         embedding_model = self._get_embedding_model(model)
         client = self._get_client(embedding_model, provider)
 
+        input_tokens = sum(client.count_string_tokens(text, embedding_model, False) for text in input_texts)
+        cost = embeddings_request_cost(embedding_model, input_tokens)
+        if cost is not None:
+            self._total_cost += cost
+
         return client.get_embeddings_sync(input_texts, embedding_model.name)
 
-    def _get_transcription_model(self, model: Model | str) -> TranscriptionModel | UnknownModel:
+    def _get_transcription_model(self, model: Model | str) -> TranscriptionModel:
         if self._model_aliases is not None and model in self._model_aliases:
             model = self._model_aliases[model]
 
         if isinstance(model, str):
             model = get_model_from_name(model)
 
-        if not isinstance(model, (TranscriptionModel, UnknownModel)):
+        if not isinstance(model, TranscriptionModel):
             raise InvalidModelError(f"Model {model} is not a transcription model")
 
         return model
 
     async def get_transcription(
         self,
-        audio_path: Path,
+        audio_path: Path | str,
         model: TranscriptionModel | str,
         provider: Optional[Provider | str] = None,
     ) -> str:
         """
         Asynchronously retrieves embeddings for a list of text.
 
         Args:
@@ -418,11 +452,18 @@
 
             model: The model to use. Must be a transciption model. If the model is unknown to Spice, a provider must be given.
             Will raise an InvalidModelError if the model is not a transciption model, or if the model is unknown and no provider was given.
 
             provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
         """
 
-        transciption_model = self._get_transcription_model(model)
-        client = self._get_client(transciption_model, provider)
+        transcription_model = self._get_transcription_model(model)
+        client = self._get_client(transcription_model, provider)
+
+        transcription, input_length = await client.get_transcription(
+            Path(audio_path).expanduser().resolve(), transcription_model.name
+        )
+        cost = transcription_request_cost(transcription_model, input_length)
+        if cost is not None:
+            self._total_cost += cost
 
-        return await client.get_transcription(audio_path, transciption_model.name)
+        return transcription
```

### Comparing `spiceai-0.1.8/LICENSE` & `spiceai-0.1.9/LICENSE`

 * *Files identical despite different names*

