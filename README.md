# 🧪 LAB 04: Provisionamento de Redes AWS (VPC) & Álgebra de Tensores para IA

## 🎯 Objetivo do Lab
Unir os fundamentos de computação em nuvem AWS (redes e segurança) com o rigor matemático de álgebra linear necessário para manipular tensores de IA.

---

## 📋 Pré-requisitos
- Ter concluído *AWS Cloud Technical Essentials* (AWS) e *Mathematics for Machine Learning* (Imperial College).
- AWS CLI v2, Python 3.10+, NumPy.

---

## 🛠️ O que você deve construir neste Lab:

### Etapa 1: Arquitetura de Nuvem AWS
1. Escreva um script em AWS CLI (`scripts/setup_vpc.sh`) que crie:
   - Uma VPC (`10.0.0.0/16`).
   - Duas subredes: uma pública (`10.0.1.0/24`) e uma privada (`10.0.2.0/24`).
   - Um Internet Gateway e tabela de roteamento.
   - Um Security Group permitindo SSH (`22`) e tráfego HTTPS (`443`).

### Etapa 2: Álgebra Matricial de Atenção (NumPy)
1. Escreva um módulo Python `math_engine/attention.py` que implemente a equação de Scaled Dot-Product Attention:
   $$	ext{Attention}(Q, K, V) = 	ext{softmax}\left(rac{QK^T}{\sqrt{d_k}}ight)V$$
2. Calcule e exiba as dimensões exatas de tensores para um modelo de dimensão $d_{model} = 4096$ e $h = 32$ cabeças de atenção.

---

## ✅ Critérios de Aceitação & Entrega
- [ ] Script AWS CLI capaz de provisionar a VPC na AWS sem erros.
- [ ] Testes unitários validando o cálculo da matriz de atenção em NumPy comparado com PyTorch.
