<!-- DECISIONS.md | Atualizado em: 16-10-2026 17:18:43(GMT-04:00) -->
# 🏛️ Decisões de Arquitetura e Governança Consolidadas (ADRs)

**Data/Hora de Geração:** `16-10-2026 17:18:43(GMT-04:00)` | **Fuso Horário:** America/Cuiaba `(GMT-04:00)`

| ID | Categoria | Decisão | Racional | Máquina | Data |
|---|---|---|---|---|---|
| `84ced170` | `ARQUITETURA` | Adoção do qwen2.5:3b como OLLAMA_REASONING_MODEL padrão no ambiente local com GTX 1060 6GB. | Consome apenas 2.9 GB de VRAM, opera 100% na GPU sem CPU offloading e funciona no Ollama 0.5.12 sem erro de tensores. | `17a6f667` | 12-10-2026 21:23:00(GMT-04:00) |
| `8a46c497` | `ARQUITETURA` | Implementação do TasksEvaluator em modo 1-a-1 atômico com varredura completa e tabela consolidada de suggested_fix. | Elimina lost-in-the-middle e complacência autorregressiva, entregando lista completa de correções de uma só vez. | `17a6f667` | 12-10-2026 21:23:00(GMT-04:00) |
| `ea9ce99b` | `ARQUITETURA` | Governança graduada de avisos onde WARN com warn_severity EXTREME é elevado programaticamente para BLOCK (exit code 1). | Impede que violações severas de arquitetura passem despercebidas como simples avisos cosméticos. | `17a6f667` | 12-10-2026 21:23:00(GMT-04:00) |
