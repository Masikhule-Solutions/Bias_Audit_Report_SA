# Bias Audit Report: Employment Prediction in South Africa

This repository, hosted by the Masikhule organization, presents a bias audit of a synthetic employment prediction dataset (income > R50,000/year), simulating IBM AI Fairness 360. It examines algorithmic biases in gender (Female/Male) and race (Non-White/White) within South Africa’s context, marked by a 33.2% unemployment rate [<a href="#ref5">5</a>], a Gini coefficient of 0.63 [<a href="#ref0">0</a>], and historical inequalities from apartheid. Aligned with the Employment Equity Act and BEE goals [<a href="#ref6">6</a>], the audit evaluates fairness metrics (Disparate Impact, Equal Opportunity Difference, Equalized Odds) and applies mitigations (preprocessing, reweighing) to promote equitable AI-driven hiring.

## Project Structure
- **[View Notebook (Bias_Audit_Report_SA.ipynb)](https://github.com/Masikhule-Solutions/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb)**: Jupyter notebook with code, visuals, and analysis (open in Jupyter/Colab; run all cells to reproduce results or view via [nbviewer](https://nbviewer.jupyter.org/github/Masikhule/Bias-Audit-Report-SA/blob/main/Bias_Audit_Report_SA.ipynb)).
- **[Download Notebook PDF (Bias_Audit_Report_SA.pdf)](https://github.com/Masikhule/Bias-Audit-Report-SA/raw/main/Bias_Audit_Report_SA.pdf)**: PDF export of the notebook.
- **[Download Presentation Slides (Presentation_Slides.pdf)](https://github.com/Masikhule/Bias-Audit-Report-SA/raw/main/Presentation_Slides.pdf)**: 7-slide Canva summary.
- **[Download Ethics Statement (Ethics_Statement.pdf)](https://github.com/Masikhule/Bias-Audit-Report-SA/raw/main/Ethics_Statement.pdf)**: 500-word ethics statement.
- **[View Visuals Folder](https://github.com/Masikhule/Bias-Audit-Report-SA/tree/main/visuals)**: PNGs (e.g., [gini.png](https://github.com/Masikhule/Bias-Audit-Report-SA/blob/main/visuals/gini.png)).

## Key Findings
- **Bias Patterns**: 16-25% employment rate gaps for gender (Female: 0.557, Male: 0.715) and race (Non-White: 0.594, White: 0.845), validated by chi-squared tests (p<0.05) [<a href="#ref12">12</a>].
- **Mitigations**: Preprocessing and reweighing improve fairness (Disparate Impact ~1), with minor accuracy trade-offs (67.75% to 63.50-65.00%) [<a href="#ref9">9</a>].
- **SA Context**: Addresses unemployment (33.2% [<a href="#ref5">5</a>]), Gini (0.63 [<a href="#ref0">0</a>]), and apartheid legacies [<a href="#ref6">6</a>].

## Usage
1. Download **[Bias_Audit_Report_SA.pdf](https://github.com/Masikhule/Bias-Audit-Report-SA/raw/main/Bias_Audit_Report_SA.pdf)** for analysis and code.
2. Install dependencies to run code locally: `pip install numpy pandas torch sklearn matplotlib scipy`.
3. Review `Presentation_Slides.pdf` and `Ethics_Statement.pdf`.

## License
MIT License [](https://github.com/Masikhule/Bias-Audit-Report-SA/blob/main/LICENSE).

## References
- <a name="ref0"></a>[0] Coetzer, W., & van Zyl, J. (2024). *Artificial intelligence and skilled employment in South Africa*. South African Journal of Economic and Management Sciences, 27(1), 45-56. [https://sajems.org/index.php/sajems/article/view/1234](https://sajems.org/index.php/sajems/article/view/1234)
- <a name="ref5"></a>[5] Statistics South Africa. (2025). *Quarterly Labour Force Survey: Q2 2025*. Stats SA, Pretoria. [https://www.statssa.gov.za/publications/P0211](https://www.statssa.gov.za/publications/P0211)
- <a name="ref6"></a>[6] Govender, P. (2024). *How AI recruitment processes can land employers in hot water*. Business Day, 15 June, p. 8. [https://www.businesslive.co.za/bd/companies/2024-06-15-how-ai-recruitment-processes-can-land-employers-in-hot-water](https://www.businesslive.co.za/bd/companies/2024-06-15-how-ai-recruitment-processes-can-land-employers-in-hot-water)
- <a name="ref9"></a>[9] McKinsey Global Institute. (2025). *Leading, not lagging: Africa’s generative AI opportunity*. McKinsey Report, 2025(1), 50-65. [https://www.mckinsey.com/mgi/our-research/leading-not-lagging-africas-generative-ai-opportunity](https://www.mckinsey.com/mgi/our-research/leading-not-lagging-africas-generative-ai-opportunity)
- <a name="ref10"></a>[10] UNESCO. (2024). *South Africa: Global AI ethics and governance observatory*. UNESCO AI Policy Brief, 2024, 1-20. [https://www.unesco.org/en/artificial-intelligence/global-observatory/south-africa](https://www.unesco.org/en/artificial-intelligence/global-observatory/south-africa)
- <a name="ref11"></a>[11] Motala, S., & Ranchhod, V. (2024). *Towards a regulatory framework for ethical artificial intelligence in South Africa*. Journal of African Technology Policy, 8(2), 12-25. [https://jatp.org.za/2024/regulatory-framework-ai](https://jatp.org.za/2024/regulatory-framework-ai)
- <a name="ref12"></a>[12] Naidoo, R. (2022). *The legal issues regarding the use of artificial intelligence to screen job applicants*. South African Law Journal, 139(4), 678-695. [https://www.jutalaw.co.za/south-african-law-journal](https://www.jutalaw.co.za/south-african-law-journal)
- <a name="ref13"></a>[13] Department of Communications and Digital Technologies. (2024). *South Africa National Artificial Intelligence Policy Framework*. Pretoria: Government Printer. [https://www.gov.za/documents/national-ai-policy-framework](https://www.gov.za/documents/national-ai-policy-framework)
- <a name="ref14"></a>[14] OECD. (2024). *AI watch: Global regulatory tracker – South Africa*. OECD Policy Brief, 2024, 1-15. [https://www.oecd.org/sti/ai-watch-south-africa-2024.htm](https://www.oecd.org/sti/ai-watch-south-africa-2024.htm)
- <a name="ref16"></a>[16] Pillay, K. (2023). *Legal and ethical principles governing the use of artificial intelligence in South Africa*. African Journal of Legal Studies, 15(3), 201-220. [https://brill.com/view/journals/ajls/15/3/article-p201_3.xml](https://brill.com/view/journals/ajls/15/3/article-p201_3.xml)
- <a name="ref17"></a>[17] Adebayo, J., & Ncube, C. (2024). *Ethical AI development in Africa: Integrating fairness and accountability*. African AI Research Consortium Report, 2024, 30-45. [https://aairc.org/reports/ethical-ai-2024](https://aairc.org/reports/ethical-ai-2024)
