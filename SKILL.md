# resume-diagnoser

Analyze a resume (PDF or text) and return a structured diagnostic report.

## Usage

```
/resume-diagnoser [path-to-resume]
```

## What it does

1. Reads the resume file provided by the user
2. Identifies strengths, weaknesses, and missing sections
3. Checks formatting, keyword density, and ATS compatibility
4. Returns a prioritized list of improvements

## Output format

- **Score**: overall resume score (0–100)
- **Strengths**: what is working well
- **Weaknesses**: what needs improvement
- **Missing sections**: expected sections that are absent
- **ATS issues**: keywords or formatting that may hurt automated screening
- **Action items**: ranked list of concrete fixes
