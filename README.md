<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Florida Nursing & Healthcare Graduate Pathways</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 20px;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
        }
        
        h1 {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-align: center;
            margin-bottom: 10px;
            font-size: 2.5em;
        }
        
        .subtitle {
            text-align: center;
            color: #666;
            margin-bottom: 40px;
            font-size: 1.1em;
        }
        
        .degree-section {
            margin-bottom: 50px;
            border-left: 5px solid #667eea;
            padding-left: 20px;
            background: linear-gradient(to right, rgba(102, 126, 234, 0.05), transparent);
            padding: 25px;
            border-radius: 10px;
        }
        
        .degree-section:nth-child(2) {
            border-left-color: #f093fb;
            background: linear-gradient(to right, rgba(240, 147, 251, 0.05), transparent);
        }
        
        .degree-section:nth-child(3) {
            border-left-color: #4facfe;
            background: linear-gradient(to right, rgba(79, 172, 254, 0.05), transparent);
        }
        
        .degree-section:nth-child(4) {
            border-left-color: #43e97b;
            background: linear-gradient(to right, rgba(67, 233, 123, 0.05), transparent);
        }
        
        h2 {
            color: #333;
            margin-bottom: 25px;
            font-size: 2em;
            padding-bottom: 10px;
            border-bottom: 3px solid;
            display: inline-block;
        }
        
        .degree-section:nth-child(1) h2 {
            border-bottom-color: #667eea;
        }
        
        .degree-section:nth-child(2) h2 {
            border-bottom-color: #f093fb;
        }
        
        .degree-section:nth-child(3) h2 {
            border-bottom-color: #4facfe;
        }
        
        .degree-section:nth-child(4) h2 {
            border-bottom-color: #43e97b;
        }
        
        .university-card {
            background: white;
            border-radius: 15px;
            padding: 25px;
            margin-bottom: 20px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 2px solid #e0e0e0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.08);
        }
        
        .university-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.15);
        }
        
        .degree-section:nth-child(1) .university-card {
            border-top: 4px solid #667eea;
        }
        
        .degree-section:nth-child(2) .university-card {
            border-top: 4px solid #f093fb;
        }
        
        .degree-section:nth-child(3) .university-card {
            border-top: 4px solid #4facfe;
        }
        
        .degree-section:nth-child(4) .university-card {
            border-top: 4px solid #43e97b;
        }
        
        h3 {
            color: #333;
            margin-bottom: 15px;
            font-size: 1.5em;
            font-weight: 600;
        }
        
        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-bottom: 15px;
        }
        
        .info-item {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 15px;
            border-radius: 10px;
            border-left: 4px solid;
            transition: transform 0.2s ease;
        }
        
        .info-item:hover {
            transform: translateX(5px);
        }
        
        .degree-section:nth-child(1) .info-item {
            border-left-color: #667eea;
        }
        
        .degree-section:nth-child(2) .info-item {
            border-left-color: #f093fb;
        }
        
        .degree-section:nth-child(3) .info-item {
            border-left-color: #4facfe;
        }
        
        .degree-section:nth-child(4) .info-item {
            border-left-color: #43e97b;
        }
        
        .info-label {
            font-weight: bold;
            color: #555;
            font-size: 0.9em;
            margin-bottom: 5px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        
        .info-value {
            color: #333;
            font-size: 1.1em;
            font-weight: 600;
        }
        
        .careers {
            background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%);
            padding: 20px;
            border-radius: 10px;
            margin-top: 15px;
            border-left: 4px solid #ff6b6b;
        }
        
        .careers h4 {
            color: #d63031;
            margin-bottom: 12px;
            font-size: 1.1em;
        }
        
        .careers ul {
            list-style-position: inside;
            color: #333;
        }
        
        .careers li {
            margin-bottom: 6px;
            padding-left: 5px;
        }
        
        .careers li::marker {
            color: #ff6b6b;
        }
        
        .program-link {
            display: inline-block;
            margin-top: 15px;
            padding: 12px 25px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            text-decoration: none;
            border-radius: 25px;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(102, 126, 234, 0.3);
        }
        
        .program-link:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 20px rgba(102, 126, 234, 0.4);
        }
        
        .degree-section:nth-child(2) .program-link {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            box-shadow: 0 4px 15px rgba(240, 147, 251, 0.3);
        }
        
        .degree-section:nth-child(2) .program-link:hover {
            box-shadow: 0 6px 20px rgba(240, 147, 251, 0.4);
        }
        
        .degree-section:nth-child(3) .program-link {
            background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
            box-shadow: 0 4px 15px rgba(79, 172, 254, 0.3);
        }
        
        .degree-section:nth-child(3) .program-link:hover {
            box-shadow: 0 6px 20px rgba(79, 172, 254, 0.4);
        }
        
        .degree-section:nth-child(4) .program-link {
            background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);
            box-shadow: 0 4px 15px rgba(67, 233, 123, 0.3);
        }
        
        .degree-section:nth-child(4) .program-link:hover {
            box-shadow: 0 6px 20px rgba(67, 233, 123, 0.4);
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 20px;
            }
            
            h1 {
                font-size: 1.8em;
            }
            
            h2 {
                font-size: 1.5em;
            }
            
            .info-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎓 Florida Nursing & Healthcare Graduate Pathways</h1>
        <p class="subtitle">Comprehensive Guide to Advanced Nursing Education in Florida</p>
        
        <!-- MSN Section -->
        <div class="degree-section">
            <h2>Master of Science in Nursing (MSN)</h2>
            
            <div class="university-card">
                <h3>University of Central Florida (UCF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">36-45</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">2-3 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$15,000-$25,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Nurse Practitioner (FNP, AGACNP, PMHNP)</li>
                        <li>Clinical Nurse Specialist</li>
                        <li>Nurse Educator</li>
                        <li>Nurse Administrator</li>
                    </ul>
                </div>
                <a href="https://nursing.ucf.edu/msn/" class="program-link" target="_blank">Visit Program →</a>
            </div>
            
            <div class="university-card">
                <h3>University of South Florida (USF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">39-47</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">2-3 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$16,000-$28,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Advanced Practice Registered Nurse (APRN)</li>
                        <li>Nurse Practitioner (various specialties)</li>
                        <li>Clinical Nurse Leader</li>
                        <li>Healthcare Administrator</li>
                    </ul>
                </div>
                <a href="https://www.usf.edu/nursing/graduate/msn/index.aspx" class="program-link" target="_blank">Visit Program →</a>
            </div>
            
            <div class="university-card">
                <h3>Florida Atlantic University (FAU)</h3>
                <div class="grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">36-48</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">2-3 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$14,000-$24,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Family Nurse Practitioner</li>
                        <li>Adult-Gerontology Nurse Practitioner</li>
                        <li>Psychiatric Mental Health Nurse Practitioner</li>
                        <li>Nurse Anesthetist (CRNA pathway)</li>
                    </ul>
                </div>
                <a href="https://www.fau.edu/nursing/graduate-programs/msn/" class="program-link" target="_blank">Visit Program →</a>
            </div>
        </div>
        
        <!-- DNP Section -->
        <div class="degree-section">
            <h2>Doctor of Nursing Practice (DNP)</h2>
            
            <div class="university-card">
                <h3>University of Central Florida (UCF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">75-80 (BSN-DNP)</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">3-4 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$30,000-$45,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Advanced Practice Nurse Leader</li>
                        <li>Clinical Director</li>
                        <li>Healthcare System Administrator</li>
                        <li>Policy Advocate</li>
                        <li>Clinical Researcher</li>
                    </ul>
                </div>
                <a href="https://nursing.ucf.edu/dnp/" class="program-link" target="_blank">Visit Program →</a>
            </div>
            
            <div class="university-card">
                <h3>University of South Florida (USF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">73-78 (BSN-DNP)</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">3-5 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$32,000-$48,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Executive Nurse Leader</li>
                        <li>Chief Nursing Officer</li>
                        <li>Healthcare Consultant</li>
                        <li>Quality Improvement Director</li>
                        <li>Advanced Clinical Practitioner</li>
                    </ul>
                </div>
                <a href="https://www.usf.edu/nursing/graduate/dnp/index.aspx" class="program-link" target="_blank">Visit Program →</a>
            </div>
            
            <div class="university-card">
                <h3>University of Florida (UF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">76-82 (BSN-DNP)</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">3-4 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$35,000-$50,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Nurse Executive</li>
                        <li>Healthcare Innovation Leader</li>
                        <li>Population Health Manager</li>
                        <li>Clinical Systems Director</li>
                        <li>Advanced Practice Provider</li>
                    </ul>
                </div>
                <a href="https://nursing.ufl.edu/academics/doctor-of-nursing-practice-dnp/" class="program-link" target="_blank">Visit Program →</a>
            </div>
        </div>
        
        <!-- PhD Section -->
        <div class="degree-section">
            <h2>PhD in Nursing</h2>
            
            <div class="university-card">
                <h3>University of Florida (UF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">90 minimum</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">4-5 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">Often funded</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Nurse Scientist/Researcher</li>
                        <li>University Professor</li>
                        <li>Research Director</li>
                        <li>Policy Researcher</li>
                        <li>Academic Dean</li>
                    </ul>
                </div>
                <a href="https://nursing.ufl.edu/academics/phd-in-nursing-science/" class="program-link" target="_blank">Visit Program →</a>
            </div>
            
            <div class="university-card">
                <h3>University of South Florida (USF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">72-90</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">4-6 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">Assistantships available</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Nursing Faculty</li>
                        <li>Clinical Research Scientist</li>
                        <li>Healthcare Policy Analyst</li>
                        <li>Postdoctoral Researcher</li>
                        <li>Academic Administrator</li>
                    </ul>
                </div>
                <a href="https://www.usf.edu/nursing/graduate/phd/index.aspx" class="program-link" target="_blank">Visit Program →</a>
            </div>
            
            <div class="university-card">
                <h3>University of Central Florida (UCF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">66-75</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">4-5 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">Funding opportunities</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Nurse Educator</li>
                        <li>Research Investigator</li>
                        <li>Health Services Researcher</li>
                        <li>Academic Leader</li>
                        <li>Grant Writer/Principal Investigator</li>
                    </ul>
                </div>
                <a href="https://nursing.ucf.edu/phd/" class="program-link" target="_blank">Visit Program →</a>
            </div>
        </div>
        
        <!-- MHA Section -->
        <div class="degree-section">
            <h2>Master of Healthcare Administration (MHA)</h2>
            
            <div class="university-card">
                <h3>University of Florida (UF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">60</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">2 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$30,000-$40,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Hospital Administrator</li>
                        <li>Healthcare Operations Manager</li>
                        <li>Clinical Director</li>
                        <li>Health Services Manager</li>
                        <li>Healthcare Consultant</li>
                    </ul>
                </div>
                <a href="https://mha.phhp.ufl.edu/" class="program-link" target="_blank">Visit Program →</a>
            </div>
            
            <div class="university-card">
                <h3>University of South Florida (USF)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">48-54</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">2 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$25,000-$35,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Healthcare Executive</li>
                        <li>Medical Practice Manager</li>
                        <li>Health Policy Analyst</li>
                        <li>Quality Improvement Director</li>
                        <li>Healthcare Finance Manager</li>
                    </ul>
                </div>
                <a href="https://www.usf.edu/business/graduate/mha/" class="program-link" target="_blank">Visit Program →</a>
            </div>
            
            <div class="university-card">
                <h3>Florida International University (FIU)</h3>
                <div class="info-grid">
                    <div class="info-item">
                        <div class="info-label">Credits</div>
                        <div class="info-value">42-48</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Length</div>
                        <div class="info-value">2 years</div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Estimated Tuition</div>
                        <div class="info-value">$22,000-$32,000</div>
                    </div>
                </div>
                <div class="careers">
                    <h4>Career Outcomes:</h4>
                    <ul>
                        <li>Healthcare Administrator</li>
                        <li>Hospital Department Director</li>
                        <li>Healthcare Strategy Consultant</li>
                        <li>Long-term Care Administrator</li>
                        <li>Public Health Manager</li>
                    </ul>
                </div>
                <a href="https://business.fiu.edu/graduate/masters-programs/healthcare-mba/index.html" class="program-link" target="_blank">Visit Program →</a>
            </div>
        </div>
        
    </div>
</body>
</html>
