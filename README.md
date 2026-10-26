# Студия Димитър Еленов, редизайн с AI чат

Структура: public/index.html (сайтът), worker.js (чат и заявки), wrangler.jsonc.

## Пускане (Cloudflare)
1. npm i -g wrangler && wrangler login
2. wrangler secret put GEMINI_API_KEY   (или ANTHROPIC_API_KEY / OPENAI_API_KEY / XAI_API_KEY, стига един)
3. wrangler deploy

Незадължително: KV binding LEADS (запис на заявки) и променлива LEAD_WEBHOOK (изпращане на заявки към имейл/CRM).
Ако чатът няма ключ или сървър, работи скриптиран резервен режим.
Снимките на преподавателите се зареждат от dimitarelenov.bg, за финална версия ги сложете в public/images.
