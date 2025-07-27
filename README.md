# 🗳️ Sistema de Votação em Assembly x86

Sistema simples de votação desenvolvido em Assembly x86 (32-bit) para Linux

## 📋 Pré-requisitos
- Linux (ou WSL no Windows)
- NASM instalado
- GNU Linker (ld)

## ⚙️ Como compilar e executar

```bash
# Instalar dependências
sudo apt-get install nasm gcc-multilib

# Compilar
nasm -f elf32 voting_system.asm -o voting.o
ld -m elf_i386 voting.o -o voting

# Executar
./voting
