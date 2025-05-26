# UnInspector for Omni Networking

A modern, extensible Inspector and serialization toolkit for Unity — **official fork of Tri-Inspector, mantido e evoluído para o ecossistema Omni Networking**.

---

## 🚀 Overview

**UnInspector** é um fork avançado do [Tri-Inspector](https://github.com/codewriter-packages/Tri-Inspector), atualizado especialmente para uso com o framework [Omni Networking](https://github.com/seu-omni-networking-link).

Potencialize seu Inspector e a serialização no Unity com novos atributos, suporte nativo a dicionários observáveis/serializáveis, e várias correções de bugs para projetos multiplayer de alto desempenho.

---

## ✨ Principais Diferenciais

- **Integração oficial com Omni Networking**  
  Fluxo de trabalho otimizado para projetos multiplayer e networked.
- **Correções de bugs & melhorias de estabilidade**  
  Compatibilidade aprimorada para Unity 2022+ e .NET modernos.
- **Novos atributos de Inspector**  
  Atributos exclusivos para dados de rede e coleções observáveis.
- **ObservableDictionary serializável**  
  Suporte total a dicionários observáveis com serialização e eventos de mudança em runtime.
- **Compatível com projetos antigos**  
  Pode substituir Tri-Inspector em projetos existentes sem retrabalho.

---

## 📚 Exemplos de Uso

#### Observable Dictionary serializável

```csharp
using Omni.Inspector;
using Omni.Collections;
using UnityEngine;

public class PlayerStats : MonoBehaviour
{
    public ObservableDictionary<string, int> Stats = new();
}
