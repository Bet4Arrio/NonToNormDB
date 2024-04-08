



- [ ] DataBase
	- [x] Baixar
	- [ ] FIltragem Dados
- [ ] Extracao
	- [ ] SIFT
	- [ ] Textura
	- [ ] Cor
	- [ ] Geometria
	- [ ] forma
- [ ] Alg-medir
	- [ ] Tempo
	- [ ] Memoria
- [ ] Treino
	- [ ] CNN
	- [ ] SVM
- [ ] Geral
	- [ ] Introducao
		- [x] base
		- [ ] Final
	- [ ] Revisao
		- [x] base
		- [ ] final
	- [ ] Meterias e metodos
		- [ ] base
		- [ ] final
- [ ] Resultados
	- [ ] analise acuraria
	- [ ] analise tempo
	- [ ] analise memoria

```mermaid
gantt
    title Tarefas PLP
    dateFormat YYYY-MM-DD
    section Databese
        Baixar Database       :a1, 2024-04-08, 1d
        Filtragem de datos   :a2, after a1, 7d
    section Extração
        Extração-SIFT : e1, after a2, 2d
        Extração-TExtura : e2, after a2, 2d
        Extração-Cor : e3, after a2, 2d
        Extração-Geometria : e4, after a2, 2d
        Extração-forma : e5, after a2, 2d
        juntar todas :ef, after e5, 7d
    section Medicao
	    medir-tempo : m1, after a2, 3d
	    medir-memoria : m2, after m1, 3d
	    decorator de medicao : m3, after m2, 
    section Treino-Classificacao
	    Treinar-CNN :after a2 m2, 7d
	    Treinar-svm-Linear :T1, after ef m2 , 7d
	section Resultado
		tabela-acuraria: after T1, 1d
		tabela-tempo: after T1, 1d
		tabela-memoria: after T1, 1d
		
	section Geral
		Rescrita-Introducao:g1, 2024-04-15, 7d
		Rescrita-revisao:g2, after g1, 7d
		escrita-materiaisEmetodos:g3, after g2, 7d
	section Extra
		tabela-wats: after T1, 1d
```


