# Pre-requisites
1. Make 2 new files and name them 'apikey.txt' and 'mongodb_key.txt'.
2. Paste your OpenAI API key in the 'apikey.txt' file.
3. Paste your MongoDB connection URI in the 'mongodb_key.txt' file.
4. Go to your MongoDB account and create a database named healthcare.
5. Create 4 collections called 'employees', 'hospital', 'emp' and 'hsp'.
6. Go to the Atlas Vector Search and create 2 vector search indices for the 'emp' and 'hsp' collections, name them 'emp_index' and 'hsp_index' respectively.
7. Paste the following in the editor for both the indices:
'''bash
{
  "fields": [
    {
      "numDimensions": 1536,
      "path": "embedding",
      "similarity": "cosine",
      "type": "vector"
    }
  ]
}
'''
