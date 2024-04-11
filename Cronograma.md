

```mermaid
gantt
    title Tarefas PLP
    tickInterval 1week 

    dateFormat YYYY-MM-DD
    section Databese
        Baixar Database       :a1, 2024-04-08, 1d
        Filtragem de datos   :a2, after a1, 7d
    section Codigos
        Extração-SIFT : e1, after a2, 2d
        Extração-TExtura : e2, after e1, 2d
        Extração-Cor : e3, after e1, 2d
        Extração-Geometria : e4, after e3, 2d
        Extração-forma : e5, after e3, 2d
        FuncaoGeral :e6, after e5, 3d
        representacaoVetor :ef, after e6, 3d
	    metodos-medir-tempo : m1, after a2, 3d
	    metodos-medir-memoria : m2, after m1, 3d
	    decorator de medicao : m3, after m2, 3d
	    implementar-SVM-linear:  IA2, after ef, 7d
	    implementar-AlexNew:  IA1, after m3, 7d
    section Treino-Classificacao
	    Treinar-CNN : TIA1, after IA1, 7d
	    Treinar-svm-Linear : TIA2, after IA2 , 7d
	    
	section Resultado
		tabela-acuraria: r1, after TIA1 TIA2, 1d
		tabela-tempo: r2,after r1, 1d
		tabela-memoria: r3, after r2, 1d
		
	section Geral
		Rescrita-Introducao:g1, after IA1, 7d
		Rescrita-revisao:g2, after g1, 7d
		escrita-materiaisEmetodos:g3, after g2, 7d
		escrita-conclusão:g4, after g3 r3, 7d
	section Apresentaca
		Gravar-video: after g4, 1d
```




## Tabela de Resposabilidade




| Section              | Tarefa                    | Emanuel | Jose | feito |
| -------------------- | ------------------------- | ------- | ---- | ----- |
| Databese             | Baixar Database           | [x]     | [ ]  |  x    |
| Databese             | Filtragem de datos        | [x]     | [x]  |       |
| Codigos              | Extração-SIFT             | []      | [x]  |       |
| Codigos              | Extração-Textura          | []      | [x]  |       |
| Codigos              | Extração-Cor              | []      | [x]  |       |
| Codigos              | Extração-Geometria        | [x]     | []   |       |
| Codigos              | Extração-forma            | [x]     | []   |       |
| Codigos              | FuncaoGeral               | [x]     | [x]  |       |
| Codigos              | representacaoVetor        | [x]     | [x]  |       |
| Codigos              | metodos-medir-tempo       | []      | [x]  |       |
| Codigos              | metodos-medir-memoria     | [x]     | []   |       |
| Codigos              | decorator de medicao      | [x]     | []   |       |
| Codigos              | implementar-SVM-linear    | []      | [x]  |       |
| Codigos              | implementar-AlexNew       | [x]     | []   |       |
| Treino-Classificacao | Treinar-CNN               | [x]     | []   |       |
| Treino-Classificacao | Treinar-svm-Linea         | [x]     | []   |       |
| Resultado            | tabela-acuraria           | [x]     | [x]  |       |
| Resultado<br>        | tabela-tempo              | [x]     | [x]  |       |
| Resultado            | tabela-memoria            | [x]     | [x]  |       |
| Geral                | Rescrita-Introducao       | [ ]     | [x]  |       |
| Geral                | Rescrita-revisao          | [ ]     | [x]  |       |
| Geral                | escrita-materiaisEmetodos | [ ]     | [x]  |       |
| Geral                | escrita-conclusão         | [x]     | [x]  |       |
| Apresentaca          | Gravar-video              | [x]     | [x]  |       |


### Lista de Feito

- [ ] Tudo
	- [ ] Database
		- [x] Baixar
		- [ ] Filtrar
	- [ ] Codigos
		- [ ] SIFT
		- [ ] Cor
		- [ ] Textura
		- [ ] Geometria
		- [ ] forma
		- [ ] Func geral
		- [ ] Representacao Vetor
		- [ ] medir-tempo
		- [ ] medir-memoria
		- [ ] Decorator
		- [ ] SVM
		- [ ] AlexNet
	- [ ] Treino-classifcacao
		- [ ] SVM
		- [ ] AlexNet
	- [ ] Resultado
		- [ ] acc
		- [ ] tempo
		- [ ] memoria
	- [ ] Geral
		- [ ] Introducão
		- [ ] revisão
		- [ ] meterias e metoods
		- [ ] conclsuão
	- [ ] Apresentacao
		- [ ] gravar
		- [ ] editar
		- [ ] publicar