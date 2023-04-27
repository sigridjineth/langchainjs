---
title: "ChatConversationalAgent"
---

# ChatConversationalAgent

Agent for the MRKL chain.

## Hierarchy

- [`Agent`](Agent.md).**ChatConversationalAgent**

## Constructors

### constructor()

> **new ChatConversationalAgent**(`input`: [`ChatConversationalAgentInput`](../types/ChatConversationalAgentInput.md)): [`ChatConversationalAgent`](ChatConversationalAgent.md)

#### Parameters

| Parameter | Type                                                                       |
| :-------- | :------------------------------------------------------------------------- |
| `input`   | [`ChatConversationalAgentInput`](../types/ChatConversationalAgentInput.md) |

#### Returns

[`ChatConversationalAgent`](ChatConversationalAgent.md)

#### Overrides

[Agent](Agent.md).[constructor](Agent.md#constructor)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:46](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L46)

## Properties

### llmChain

> **llmChain**: [`LLMChain`](../../chains/classes/LLMChain.md)

#### Inherited from

[Agent](Agent.md).[llmChain](Agent.md#llmchain)

#### Defined in

[langchain/src/agents/agent.ts:199](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L199)

### outputParser

> **outputParser**: [`AgentActionOutputParser`](AgentActionOutputParser.md)

#### Inherited from

[Agent](Agent.md).[outputParser](Agent.md#outputparser)

#### Defined in

[langchain/src/agents/agent.ts:201](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L201)

## Accessors

### allowedTools

> **allowedTools**(): `undefined` \| `string`[]

#### Returns

`undefined` \| `string`[]

#### Inherited from

Agent.allowedTools

#### Defined in

[langchain/src/agents/agent.ts:205](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L205)

#### Inherited from

[Agent](Agent.md).[allowedTools](Agent.md#allowedtools)

#### Defined in

[langchain/src/agents/agent.ts:205](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L205)

### inputKeys

> **inputKeys**(): `string`[]

#### Returns

`string`[]

#### Inherited from

Agent.inputKeys

#### Defined in

[langchain/src/agents/agent.ts:209](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L209)

#### Inherited from

[Agent](Agent.md).[inputKeys](Agent.md#inputkeys)

#### Defined in

[langchain/src/agents/agent.ts:209](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L209)

### returnValues

> **returnValues**(): `string`[]

#### Returns

`string`[]

#### Inherited from

Agent.returnValues

#### Defined in

[langchain/src/agents/agent.ts:35](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L35)

#### Inherited from

[Agent](Agent.md).[returnValues](Agent.md#returnvalues)

#### Defined in

[langchain/src/agents/agent.ts:35](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L35)

## Methods

### \_agentActionType()

> **\_agentActionType**(): `string`

#### Returns

`string`

#### Inherited from

[Agent](Agent.md).[\_agentActionType](Agent.md#_agentactiontype)

#### Defined in

[langchain/src/agents/agent.ts:86](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L86)

### \_agentType()

Return the string type key uniquely identifying this class of agent.

> **\_agentType**(): "chat-conversational-react-description"

#### Returns

"chat-conversational-react-description"

#### Overrides

[Agent](Agent.md).[\_agentType](Agent.md#_agenttype)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:52](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L52)

### \_stop()

> **\_stop**(): `string`[]

#### Returns

`string`[]

#### Overrides

[Agent](Agent.md).[\_stop](Agent.md#_stop)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:64](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L64)

### constructScratchPad()

Construct a scratchpad to let the agent continue its thought process

> **constructScratchPad**(`steps`: [`AgentStep`](../../schema/types/AgentStep.md)[]): `Promise`<[`BaseChatMessage`](../../schema/classes/BaseChatMessage.md)[]\>

#### Parameters

| Parameter | Type                                             |
| :-------- | :----------------------------------------------- |
| `steps`   | [`AgentStep`](../../schema/types/AgentStep.md)[] |

#### Returns

`Promise`<[`BaseChatMessage`](../../schema/classes/BaseChatMessage.md)[]\>

#### Overrides

[Agent](Agent.md).[constructScratchPad](Agent.md#constructscratchpad)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:78](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L78)

### finishToolName()

Name of tool to use to terminate the chain.

> **finishToolName**(): `string`

#### Returns

`string`

#### Inherited from

[Agent](Agent.md).[finishToolName](Agent.md#finishtoolname)

#### Defined in

[langchain/src/agents/agent.ts:282](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L282)

### llmPrefix()

Prefix to append the LLM call with.

> **llmPrefix**(): `string`

#### Returns

`string`

#### Overrides

[Agent](Agent.md).[llmPrefix](Agent.md#llmprefix)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:60](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L60)

### observationPrefix()

Prefix to append the observation with.

> **observationPrefix**(): `string`

#### Returns

`string`

#### Overrides

[Agent](Agent.md).[observationPrefix](Agent.md#observationprefix)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:56](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L56)

### plan()

Decide what to do given some input.

> **plan**(`steps`: [`AgentStep`](../../schema/types/AgentStep.md)[], `inputs`: [`ChainValues`](../../schema/types/ChainValues.md), `callbackManager`?: [`CallbackManager`](../../callbacks/classes/CallbackManager.md)): `Promise`<[`AgentAction`](../../schema/types/AgentAction.md) \| [`AgentFinish`](../../schema/types/AgentFinish.md)\>

#### Parameters

| Parameter          | Type                                                            | Description                                                        |
| :----------------- | :-------------------------------------------------------------- | :----------------------------------------------------------------- |
| `steps`            | [`AgentStep`](../../schema/types/AgentStep.md)[]                | Steps the LLM has taken so far, along with observations from each. |
| `inputs`           | [`ChainValues`](../../schema/types/ChainValues.md)              | User inputs.                                                       |
| `callbackManager?` | [`CallbackManager`](../../callbacks/classes/CallbackManager.md) | Callback manager to use for this call.                             |

#### Returns

`Promise`<[`AgentAction`](../../schema/types/AgentAction.md) \| [`AgentFinish`](../../schema/types/AgentFinish.md)\>

Action specifying what tool to use.

#### Inherited from

[Agent](Agent.md).[plan](Agent.md#plan)

#### Defined in

[langchain/src/agents/agent.ts:333](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L333)

### prepareForOutput()

Prepare the agent for output, if needed

> **prepareForOutput**(`_returnValues`: `Record`<`string`, `any`\>, `_steps`: [`AgentStep`](../../schema/types/AgentStep.md)[]): `Promise`<`Record`<`string`, `any`\>\>

#### Parameters

| Parameter       | Type                                             |
| :-------------- | :----------------------------------------------- |
| `_returnValues` | `Record`<`string`, `any`\>                      |
| `_steps`        | [`AgentStep`](../../schema/types/AgentStep.md)[] |

#### Returns

`Promise`<`Record`<`string`, `any`\>\>

#### Inherited from

[Agent](Agent.md).[prepareForOutput](Agent.md#prepareforoutput)

#### Defined in

[langchain/src/agents/agent.ts:77](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L77)

### returnStoppedResponse()

Return response when agent has been stopped due to max iterations

> **returnStoppedResponse**(`earlyStoppingMethod`: [`StoppingMethod`](../types/StoppingMethod.md), `steps`: [`AgentStep`](../../schema/types/AgentStep.md)[], `inputs`: [`ChainValues`](../../schema/types/ChainValues.md), `callbackManager`?: [`CallbackManager`](../../callbacks/classes/CallbackManager.md)): `Promise`<[`AgentFinish`](../../schema/types/AgentFinish.md)\>

#### Parameters

| Parameter             | Type                                                            |
| :-------------------- | :-------------------------------------------------------------- |
| `earlyStoppingMethod` | [`StoppingMethod`](../types/StoppingMethod.md)                  |
| `steps`               | [`AgentStep`](../../schema/types/AgentStep.md)[]                |
| `inputs`              | [`ChainValues`](../../schema/types/ChainValues.md)              |
| `callbackManager?`    | [`CallbackManager`](../../callbacks/classes/CallbackManager.md) |

#### Returns

`Promise`<[`AgentFinish`](../../schema/types/AgentFinish.md)\>

#### Inherited from

[Agent](Agent.md).[returnStoppedResponse](Agent.md#returnstoppedresponse)

#### Defined in

[langchain/src/agents/agent.ts:344](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L344)

### createPrompt()

Create prompt in the style of the ChatConversationAgent.

> `Static` **createPrompt**(`tools`: [`Tool`](../../tools/classes/Tool.md)[], `args`?: [`ChatConversationalCreatePromptArgs`](../interfaces/ChatConversationalCreatePromptArgs.md)): [`ChatPromptTemplate`](../../prompts/classes/ChatPromptTemplate.md)

#### Parameters

| Parameter | Type                                                                                        | Description                                                             |
| :-------- | :------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------- |
| `tools`   | [`Tool`](../../tools/classes/Tool.md)[]                                                     | List of tools the agent will have access to, used to format the prompt. |
| `args?`   | [`ChatConversationalCreatePromptArgs`](../interfaces/ChatConversationalCreatePromptArgs.md) | Arguments to create the prompt with.                                    |

#### Returns

[`ChatPromptTemplate`](../../prompts/classes/ChatPromptTemplate.md)

#### Overrides

[Agent](Agent.md).[createPrompt](Agent.md#createprompt)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:107](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L107)

### deserialize()

Load an agent from a json-like object describing it.

> `Static` **deserialize**(`data`: `Object`): `Promise`<[`Agent`](Agent.md)\>

#### Parameters

| Parameter | Type     |
| :-------- | :------- |
| `data`    | `Object` |

#### Returns

`Promise`<[`Agent`](Agent.md)\>

#### Inherited from

[Agent](Agent.md).[deserialize](Agent.md#deserialize)

#### Defined in

[langchain/src/agents/agent.ts:386](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/agent.ts#L386)

### fromLLMAndTools()

Construct an agent from an LLM and a list of tools

> `Static` **fromLLMAndTools**(`llm`: [`BaseLanguageModel`](../../base_language/classes/BaseLanguageModel.md), `tools`: [`Tool`](../../tools/classes/Tool.md)[], `args`?: [`ChatConversationalCreatePromptArgs`](../interfaces/ChatConversationalCreatePromptArgs.md) & [`AgentArgs`](../interfaces/AgentArgs.md)): [`ChatConversationalAgent`](ChatConversationalAgent.md)

#### Parameters

| Parameter | Type                                                                                                                                    |
| :-------- | :-------------------------------------------------------------------------------------------------------------------------------------- |
| `llm`     | [`BaseLanguageModel`](../../base_language/classes/BaseLanguageModel.md)                                                                 |
| `tools`   | [`Tool`](../../tools/classes/Tool.md)[]                                                                                                 |
| `args?`   | [`ChatConversationalCreatePromptArgs`](../interfaces/ChatConversationalCreatePromptArgs.md) & [`AgentArgs`](../interfaces/AgentArgs.md) |

#### Returns

[`ChatConversationalAgent`](ChatConversationalAgent.md)

#### Overrides

[Agent](Agent.md).[fromLLMAndTools](Agent.md#fromllmandtools)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:135](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L135)

### getDefaultOutputParser()

Get the default output parser for this agent.

> `Static` **getDefaultOutputParser**(`_fields`?: [`OutputParserArgs`](../types/OutputParserArgs.md)): [`AgentActionOutputParser`](AgentActionOutputParser.md)

#### Parameters

| Parameter  | Type                                               |
| :--------- | :------------------------------------------------- |
| `_fields?` | [`OutputParserArgs`](../types/OutputParserArgs.md) |

#### Returns

[`AgentActionOutputParser`](AgentActionOutputParser.md)

#### Overrides

[Agent](Agent.md).[getDefaultOutputParser](Agent.md#getdefaultoutputparser)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:93](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L93)

### validateTools()

Validate that appropriate tools are passed in

> `Static` **validateTools**(`tools`: [`Tool`](../../tools/classes/Tool.md)[]): `void`

#### Parameters

| Parameter | Type                                    |
| :-------- | :-------------------------------------- |
| `tools`   | [`Tool`](../../tools/classes/Tool.md)[] |

#### Returns

`void`

#### Overrides

[Agent](Agent.md).[validateTools](Agent.md#validatetools)

#### Defined in

[langchain/src/agents/chat_convo/index.ts:68](https://github.com/hwchase17/langchainjs/blob/ddf2996/langchain/src/agents/chat_convo/index.ts#L68)