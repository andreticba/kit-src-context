<!-- LEARNINGS.md | Atualizado em: 12-10-2026 21:26:52(GMT-04:00) -->
# 💡 Aprendizados Técnicos e Lições Aprendidas Consolidadas

**Data/Hora de Geração:** `12-10-2026 21:26:52(GMT-04:00)` | **Fuso Horário:** America/Cuiaba `(GMT-04:00)`

## KIT
- **Aprendizado:** [KIT] O modelo phi4-mini exige Ollama >= 0.5.13 devido a novos tensores GGUF (missing tensor 'output.weight'). Para Ollama 0.5.12 em GPU de 6GB, o qwen2.5:3b é a alternativa ideal com 2.9GB de VRAM e suporte nativo a JSON Schema.
  - **Racional:** Garante estabilidade e agilidade de inferência sem necessitar de atualização imediata da imagem Docker do motor.
  - **Origem:** `ai-control` | **Data:** 12-10-2026 21:23:00(GMT-04:00)
- **Aprendizado:** [KIT] Constrained Grammar Decoding (format JSON Schema) com CoT invertido (critique antes de verdict) elimina sycophancy e garante determinismo sintático em 100% das chamadas locais.
  - **Racional:** Evita erros de parsing markdown e assegura que a fundamentação crítica seja gerada antes da classificação.
  - **Origem:** `ai-control` | **Data:** 12-10-2026 21:23:00(GMT-04:00)
- **Aprendizado:** [KIT] A estratégia adaptativa trifásica de auditoria (holística para spec, seções para plan e 1-a-1 com varredura completa para tasks) soluciona o gargalo do fatiamento cego por caracteres.
  - **Racional:** Cada artefato SDD possui topologia distinta de acoplamento contextual.
  - **Origem:** `ai-control` | **Data:** 12-10-2026 21:23:00(GMT-04:00)
