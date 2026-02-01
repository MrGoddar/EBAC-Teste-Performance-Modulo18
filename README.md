# EBAC - Módulo 18: Teste de Performance com JMeter

Este repositório contém os arquivos da Tarefa 18 do curso de Qualidade de Software da EBAC.

## 📋 Cenário de Teste
* **Endpoint:** www.youtube.com
* **Usuários (Threads):** 20
* **Ramp-up:** 60 segundos
* **Duração:** 3 minutos
* **Massa de Dados:** Arquivo `.csv` com 10 termos de busca

## 🛠️ Arquivos
* `exercício18.jmx`: Script de teste configurado.
* `dados - Página1.csv`: Massa de dados utilizada.

## ⚠️ Nota Técnica
Durante a execução, foi identificada uma incompatibilidade da biblioteca SIGAR (`sigar-amd64-winnt.dll`) com o Windows 11, resultando no erro `EXCEPTION_ACCESS_VIOLATION`. Por esse motivo, o monitoramento de recursos foi validado localmente, e o foco do script enviado é a carga de usuários e o tempo de resposta das requisições.
