PhD Shortlist Builder
Overview

This project builds personalized PhD supervisor recommendations from a student profile.

The system:

Discovers researchers using OpenAlex
Verifies likely supervisors
Matches research interests using semantic similarity
Generates ranked recommendations
Architecture

Student Profile
→ Research Topic Extraction
→ Candidate Discovery
→ Supervisor Verification
→ Semantic Matching
→ Ranking
→ Shortlist Generation


Installation
pip install -r requirements.txt
Usage
python run.py

Example Input
{
  "research_interests": [
    "Computer Vision",
    "Medical Imaging",
    "Deep Learning"
  ]
}

Output
{
  "recommendations": [
    {
      "name": "Professor X",
      "institution": "University Y",
      "score": 91.4
    }
  ]
}


Future Improvements

Grant discovery
Eligibility extraction
Faculty-page verification
Learning-to-rank model
OpenAI explanation generation


