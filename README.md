# Gpt.aitools.chat



## Updates

Gpt.aitools.chat will be updated over time.

Expect frequent improvements.

**Next up:**

- [ ] Delete messages
- [ ] More model settings
- [ ] Plugins

**Recent updates:**

- [x] Prompt templates (3/27/23)
- [x] Regenerate & edit responses (3/25/23)
- [x] Folders (3/24/23)
- [x] Search chat content (3/23/23)
- [x] Stop message generation (3/22/23)
- [x] Import/Export chats (3/22/23)
- [x] Custom system prompt (3/21/23)
- [x] Error handling (3/20/23)
- [x] GPT-4 support (access required) (3/20/23)
- [x] Search conversations (3/19/23)
- [x] Code syntax highlighting (3/18/23)
- [x] Toggle sidebar (3/18/23)
- [x] Conversation naming (3/18/23)
- [x] Github flavored markdown (3/18/23)
- [x] Add OpenAI API key in app (3/18/23)
- [x] Markdown support (3/17/23)

## Modifications

Modify the chat interface in `components/Chat`.

Modify the sidebar interface in `components/Sidebar`.

Modify the system prompt in `utils/index.ts`.

## Deploy

**Vercel**

Host your own live version of Gpt.aitools.chat with Vercel.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FAitoolsPro%2FGpt-aitools-chat)


**Docker**

Build locally:

```shell
docker build -t gpt-aitools-chat .
docker run -e OPENAI_API_KEY=xxxxxxxx -p 3000:3000 gpt-aitools-chat
```

如果您想从 GitHub 仓库直接 构建并运行 Docker 镜像，您可以 先克隆仓库，然后在本地构建镜像。请按照以下步骤操作：
1：在您的服务器上，克隆仓库：
git clone https://github.com/AitoolsPro/Gpt-aitools-chat.git

2：进入仓库目录：
cd Gpt-aitools-chat

3:使用 Dockerfile 构建 Docker 镜 像：
docker build -t gpt-aitools-chat .

4:运行 Docker 镜像：

docker run -e OPENAI_API_KEY=你的APIKEY -p 3000:3000 gpt-aitools-chat

```

## Running Locally

**1. Clone Repo**

```bash
git clone https://github.com/aitoolspro/gpt-aitools-chat.git
```

**2. Install Dependencies**

```bash
npm i
```

**3. Provide OpenAI API Key**

Create a .env.local file in the root of the repo with your OpenAI API Key:

```bash
OPENAI_API_KEY=YOUR_KEY
```

> You can set `OPENAI_API_HOST` where access to the official OpenAI host is restricted or unavailable, allowing users to configure an alternative host for their specific needs.

> Additionally, if you have multiple OpenAI Organizations, you can set `OPENAI_ORGANIZATION` to specify one.

**4. Run App**

```bash
npm run dev
```

**5. Use It**

You should be able to start chatting.

## Configuration

When deploying the application, the following environment variables can be set:

| Environment Variable  | Default value                  | Description                                             |
| --------------------- | ------------------------------ | ------------------------------------------------------- |
| OPENAI_API_KEY        |                                | The default API key used for authentication with OpenAI |
| DEFAULT_MODEL         | `gpt-3.5-turbo`                | The default model to use on new conversations           |
| DEFAULT_SYSTEM_PROMPT | [see here](utils/app/const.ts) | The default system prompt to use on new conversations   |
| GOOGLE_API_KEY        |                                | See [Custom Search JSON API documentation][GCSE]        |
| GOOGLE_CSE_ID         |                                | See [Custom Search JSON API documentation][GCSE]        |

If you do not provide an OpenAI API key with `OPENAI_API_KEY`, users will have to provide their own key.
If you don't have an OpenAI API key, you can get one [here](https://platform.openai.com/account/api-keys).

## Contact

艾兔思Aitools-ai终极指南。让工具成为思维的延伸！ [艾兔思Ai导航论坛网](https://www.aitools.chat/).

[GCSE]: https://developers.google.com/custom-search/v1/overview
