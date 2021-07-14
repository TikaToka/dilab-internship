. install wordnet
	import nltk
	nltk.download('wordnet')

2. Change directory for user's environment
	for Compute_IDF.py
		line 60, 88
	for AIR_evidence_retrieval_scores.py
		line 16 (glove file exists in root(Air-Retriever) folder)
	for main_MultiRC_passages_from_topN_Iterarive...
		line 15 (glove file exists in root(Air-Retriever) folder)


2. execute Compute_IDF.py
	python3 Compute_IDF.py
		output should be at root folder and name should be MultiRC_IDF_vals.json"

3. execute AIR_evidence_retrieval_scores.py
	python3 Compute_IDF.py
		output will be at ./MultiRC_BM25_vs_POCC_justification_quality_score 

4. execute main_MultiRC_passages_from_topN_Iterarive...
	python3 main_MultiRC_passages_from_topN_Iterative_alignments_PARALLEL_evidences.py
		output will be at ./MultiRC_justifications_Iterative_Alignment_CLASSIFICATION_parallel_concat_evidence_5