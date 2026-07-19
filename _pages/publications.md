<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Publications | Dr. Lijesh K. P.</title>

    <style>
        :root {
            --primary-color: #123a63;
            --secondary-color: #1e6698;
            --accent-color: #c7983e;
            --background-color: #f4f7fa;
            --card-background: #ffffff;
            --text-color: #263442;
            --muted-text: #667482;
            --border-color: #dce4eb;
            --shadow: 0 8px 24px rgba(18, 58, 99, 0.08);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: var(--background-color);
            color: var(--text-color);
            line-height: 1.65;
        }

        .site-header {
            background:
                linear-gradient(
                    135deg,
                    rgba(12, 45, 76, 0.97),
                    rgba(23, 91, 137, 0.94)
                );
            color: white;
            padding: 55px 20px;
            text-align: center;
        }

        .site-header h1 {
            font-family: Georgia, "Times New Roman", serif;
            font-size: clamp(2rem, 5vw, 3.4rem);
            margin-bottom: 10px;
        }

        .site-header p {
            max-width: 760px;
            margin: 0 auto;
            font-size: 1.05rem;
            color: rgba(255, 255, 255, 0.88);
        }

        .navigation {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(255, 255, 255, 0.97);
            border-bottom: 1px solid var(--border-color);
            box-shadow: 0 3px 12px rgba(18, 58, 99, 0.06);
        }

        .navigation-inner {
            max-width: 1180px;
            margin: 0 auto;
            padding: 14px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 20px;
        }

        .brand {
            color: var(--primary-color);
            font-weight: 700;
            text-decoration: none;
        }

        .navigation-links {
            display: flex;
            flex-wrap: wrap;
            gap: 18px;
        }

        .navigation-links a {
            color: var(--text-color);
            text-decoration: none;
            font-size: 0.94rem;
            font-weight: 600;
        }

        .navigation-links a:hover {
            color: var(--secondary-color);
        }

        main {
            max-width: 1180px;
            margin: 0 auto;
            padding: 50px 20px 80px;
        }

        .section-heading {
            margin-bottom: 30px;
        }

        .section-label {
            display: inline-block;
            margin-bottom: 9px;
            color: var(--secondary-color);
            font-size: 0.78rem;
            font-weight: 700;
            letter-spacing: 0.14em;
            text-transform: uppercase;
        }

        .section-heading h2 {
            font-family: Georgia, "Times New Roman", serif;
            color: var(--primary-color);
            font-size: clamp(2rem, 4vw, 2.8rem);
            margin-bottom: 10px;
        }

        .section-heading p {
            max-width: 780px;
            color: var(--muted-text);
        }

        .publication-controls {
            display: grid;
            grid-template-columns: minmax(0, 1fr) 180px;
            gap: 14px;
            margin-bottom: 30px;
        }

        .publication-controls input,
        .publication-controls select {
            width: 100%;
            min-height: 48px;
            padding: 11px 14px;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            background: white;
            color: var(--text-color);
            font-size: 0.95rem;
            outline: none;
        }

        .publication-controls input:focus,
        .publication-controls select:focus {
            border-color: var(--secondary-color);
            box-shadow: 0 0 0 3px rgba(30, 102, 152, 0.1);
        }

        .results-summary {
            margin-bottom: 20px;
            color: var(--muted-text);
            font-size: 0.92rem;
        }

        .year-group {
            margin-bottom: 42px;
        }

        .year-heading {
            display: flex;
            align-items: center;
            gap: 14px;
            margin-bottom: 18px;
            color: var(--primary-color);
            font-family: Georgia, "Times New Roman", serif;
            font-size: 1.75rem;
        }

        .year-heading::after {
            content: "";
            height: 1px;
            flex: 1;
            background: var(--border-color);
        }

        .publication-list {
            display: grid;
            gap: 15px;
        }

        .publication-card {
            display: grid;
            grid-template-columns: 52px minmax(0, 1fr);
            gap: 16px;
            padding: 21px;
            background: var(--card-background);
            border: 1px solid var(--border-color);
            border-left: 4px solid var(--secondary-color);
            border-radius: 10px;
            box-shadow: var(--shadow);
            transition:
                transform 0.2s ease,
                box-shadow 0.2s ease,
                border-color 0.2s ease;
        }

        .publication-card:hover {
            transform: translateY(-2px);
            border-color: #c6d7e4;
            box-shadow: 0 12px 30px rgba(18, 58, 99, 0.12);
        }

        .publication-number {
            width: 42px;
            height: 42px;
            display: grid;
            place-items: center;
            border-radius: 50%;
            background: #eaf2f8;
            color: var(--primary-color);
            font-size: 0.9rem;
            font-weight: 700;
        }

        .publication-title {
            margin-bottom: 7px;
            color: var(--primary-color);
            font-family: Georgia, "Times New Roman", serif;
            font-size: 1.08rem;
            line-height: 1.45;
        }

        .publication-authors {
            margin-bottom: 5px;
            color: var(--text-color);
            font-size: 0.94rem;
        }

        .publication-journal {
            color: var(--muted-text);
            font-size: 0.92rem;
        }

        .journal-link {
            display: inline-flex;
            align-items: center;
            gap: 7px;
            margin-top: 11px;
            padding: 7px 12px;
            border: 1px solid #bed1df;
            border-radius: 6px;
            color: var(--secondary-color);
            background: #f6fafc;
            text-decoration: none;
            font-size: 0.86rem;
            font-weight: 700;
            transition:
                color 0.2s ease,
                background 0.2s ease,
                border-color 0.2s ease;
        }

        .journal-link:hover {
            color: white;
            background: var(--secondary-color);
            border-color: var(--secondary-color);
        }

        .journal-link::after {
            content: "↗";
            font-size: 0.85rem;
        }

        .empty-state {
            padding: 35px 20px;
            text-align: center;
            background: white;
            border: 1px solid var(--border-color);
            border-radius: 10px;
            color: var(--muted-text);
        }

        .site-footer {
            background: var(--primary-color);
            color: rgba(255, 255, 255, 0.84);
            text-align: center;
            padding: 25px 20px;
            font-size: 0.9rem;
        }

        @media (max-width: 720px) {
            .navigation-inner {
                flex-direction: column;
                align-items: flex-start;
            }

            .publication-controls {
                grid-template-columns: 1fr;
            }

            .publication-card {
                grid-template-columns: 42px minmax(0, 1fr);
                padding: 17px;
            }

            .publication-number {
                width: 36px;
                height: 36px;
                font-size: 0.82rem;
            }
        }
    </style>
</head>

<body>

<header class="site-header">
    <h1>Publications</h1>
    <p>
        Peer-reviewed journal articles, invited contributions, book chapters,
        and technical publications by Dr. Lijesh K. P. and collaborators.
    </p>
</header>

<nav class="navigation">
    <div class="navigation-inner">
        <a href="#" class="brand">Dr. Lijesh K. P.</a>

        <div class="navigation-links">
            <a href="#publications">Publications</a>
        </div>
    </div>
</nav>

<main>
    <section id="publications">
        <div class="section-heading">
            <span class="section-label">Research Contributions</span>
            <h2>Complete Publication List</h2>
            <p>
                Publications are arranged by year. Use the search box to locate
                a title, author, journal, research topic, or publication year.
            </p>
        </div>

        <div class="publication-controls">
            <input
                type="search"
                id="publicationSearch"
                placeholder="Search publications..."
                aria-label="Search publications"
            >

            <select
                id="yearFilter"
                aria-label="Filter publications by year"
            >
                <option value="all">All years</option>
            </select>
        </div>

        <div class="results-summary" id="resultsSummary"></div>

        <div id="publicationContainer"></div>
    </section>
</main>

<footer class="site-footer">
    <p>
        &copy; <span id="currentYear"></span> Dr. Lijesh K. P.
        All rights reserved.
    </p>
</footer>

<script>
    const publications = [
        {
            number: 1,
            year: 2026,
            authors: "Lijesh, K. P., Mohammad Khorasani, Mohammad Rouhi Moghanlou, and Michael M. Khonsari.",
            title: "Entropy-Based Quantification of Hydrogen Embrittlement.",
            journal: "International Journal of Hydrogen Energy 251 (2026): 156097.",
            doi: "https://doi.org/10.1016/j.ijhydene.2026.156097"
        },
        {
            number: 2,
            year: 2026,
            authors: "Adibi, Noushin, Ehsan Bagheri, Lijesh K. P., Saeid Zavari, Hamed Ghadimi, Michael Khonsari, and Shengmin Guo.",
            title: "High-Frequency Fatigue, Tribological Performance, and Corrosion Resistance of Al 2050 Prepared by Additive Friction Stir Deposition.",
            journal: "The International Journal of Advanced Manufacturing Technology (2026): 1–13.",
            doi: "https://doi.org/10.1007/s00170-026-18296-y"
        },
        {
            number: 3,
            year: 2026,
            authors: "Khorasani, Mohammad, Mohammad Rouhi Moghanlou, Md Ariful Islam, Lijesh K. P., and Michael M. Khonsari.",
            title: "Damage Evolution in Metals under Uniaxial Tension: Thermodynamic Approach.",
            journal: "International Journal of Mechanical Sciences (2026): 111700.",
            doi: "https://doi.org/10.1016/j.ijmecsci.2026.111700"
        },
        {
            number: 4,
            year: 2026,
            authors: "Moghanlou, Mohammad Rouhi, Mohammad Khorasani, Lijesh K. P., and Michael M. Khonsari.",
            title: "Quantifying the Static Tensile Stress Response of Notched Steel Specimens Using the Degradation Entropy Generation (DEG) Theorem.",
            journal: "Mechanics of Materials 219 (2026): 105715.",
            doi: "https://doi.org/10.1016/j.mechmat.2026.105715"
        },
        {
            number: 5,
            year: 2026,
            authors: "Lijesh, K. P., and Michael M. Khonsari.",
            title: "Wear Maps Derived from Thermodynamic Principles.",
            journal: "Wear (2026): 206694.",
            doi: "https://doi.org/10.1016/j.wear.2026.206694"
        },
        {
            number: 6,
            year: 2026,
            authors: "Farsani, Elaheh Azizian, Lijesh K. P., and Michael M. Khonsari.",
            title: "On the Degradation of Additively Manufactured Polymers and Composites.",
            journal: "Composites Science and Technology (2026): 111547.",
            doi: "https://doi.org/10.1016/j.compscitech.2026.111547"
        },
        {
            number: 7,
            year: 2026,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "Failure Threshold Entropy and Its Application in Tribology.",
            journal: "Encyclopedia of Tribology and Lubrication. Elsevier, 2026.",
            doi: "https://doi.org/10.1016/B978-0-443-30138-4.00022-4"
        },
        {
            number: 8,
            year: 2025,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "Thermodynamic Characterization of Fretting-Induced Material Degradation Using Degradation Entropy Generation Framework.",
            journal: "Wear (2025): 206341.",
            doi: "https://doi.org/10.1016/j.wear.2025.206341"
        },
        {
            number: 9,
            year: 2025,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "Thermodynamic Framework for Characterization of Flow-Induced Corrosion.",
            journal: "Tribology International (2025): 111131.",
            doi: "https://doi.org/10.1016/j.triboint.2025.111131"
        },
        {
            number: 10,
            year: 2025,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "A Thermodynamic Framework to Rapidly Determine Remaining Discharge Time in Li-Ion Batteries.",
            journal: "Journal of Power Sources 655 (2025): 237922.",
            doi: "https://doi.org/10.1016/j.jpowsour.2025.237922"
        },
        {
            number: 11,
            year: 2025,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "A Thermodynamic Approach for the Rapid Estimation of the Remaining Time to Discharge in Li-Ion Batteries.",
            journal: "Sustainable Energy Technologies and Assessments 82 (2025): 104490.",
            doi: "https://doi.org/10.1016/j.seta.2025.104490"
        },
        {
            number: 12,
            year: 2025,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "In-Situ Monitoring of Grease Consistency.",
            journal: "Invention Disclosure 5 (2025): 100036.",
            doi: null
        },
        {
            number: 13,
            year: 2025,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "Entropy-Based Unified Theory of Failure Threshold of Degrading Systems.",
            journal: "Newton 1, no. 3 (2025): 100035.",
            doi: "https://doi.org/10.1016/j.newton.2025.100035"
        },
        {
            number: 14,
            year: 2025,
            authors: "Lokhande, Rohan, Sitesh Kumar Mishra, Deepak Ronanki, Piyush Shakya, Vimal Edachery, and Lijesh K. P.",
            title: "Review on Tribological and Vibration Aspects in Mechanical Bearings of Electric Vehicles: Effect of Bearing Current, Shaft Voltage, and Electric Discharge Material Spalling Current.",
            journal: "Lubricants 13, no. 8 (2025): 349.",
            doi: "https://doi.org/10.3390/lubricants13080349"
        },
        {
            number: 15,
            year: 2024,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "A Thermodynamic Approach for Characterizing the Degradation of Li-Ion Batteries.",
            journal: "Journal of Energy Storage 82 (2024): 110565.",
            doi: "https://doi.org/10.1016/j.est.2024.110565"
        },
        {
            number: 16,
            year: 2024,
            authors: "Lijesh, K. P., Ali Mahmoudi, and M. M. Khonsari.",
            title: "Experimentally Verified Thermodynamic Framework for Corrosion.",
            journal: "Corrosion Science 233 (2024): 112063.",
            doi: "https://doi.org/10.1016/j.corsci.2024.112063"
        },
        {
            number: 17,
            year: 2024,
            authors: "Lijesh, K. P., R. A. Miller, A. Sanford, J. Carroll, and M. M. Khonsari.",
            title: "Application of Thermodynamics to Industrial Grease Production.",
            journal: "Chemical Engineering Journal 489 (2024): 151306.",
            doi: "https://doi.org/10.1016/j.cej.2024.151306"
        },
        {
            number: 18,
            year: 2024,
            authors: "Anand, P., P. Ramkumar, K. P. Lijesh, and Vimal Edachery.",
            title: "Tribological Performance of Laser-Based Surface-Textured Nonconformal Contacts.",
            journal: "Advances in Tribology 2024 (2024).",
            doi: "https://doi.org/10.1155/2024/1424767"
        },
        {
            number: 19,
            year: 2023,
            authors: "Lijesh, K. P., Roger A. Miller, Raj Shah, Khosro Shirvani, and Michael M. Khonsari.",
            title: "The Standard for Assessing Water Resistance Properties of Lubricating Grease Using Contact Angle Measurements.",
            journal: "Lubricants 11, no. 10 (2023): 440.",
            doi: "https://doi.org/10.3390/lubricants11100440"
        },
        {
            number: 20,
            year: 2023,
            authors: "Mahmoudi, Ali, Mohammad A. Amooie, Lijesh K. P., and Michael M. Khonsari.",
            title: "In Situ Prediction of Metal Fatigue Life Using Frequency Change.",
            journal: "Metals 13, no. 10 (2023): 1681.",
            doi: "https://doi.org/10.3390/met13101681"
        },
        {
            number: 21,
            year: 2023,
            authors: "Kumar, Deepak, G. A. Harmain, Gaurav Gaurav, K. P. Lijesh, Basil Kuriachen, Harish Hirani, and Jibin T. Philip.",
            title: "A Novel Seal Design to Enhance MR Brake Performance.",
            journal: "Transactions of the Indian Institute of Metals 76, no. 9 (2023): 2335–2342.",
            doi: "https://doi.org/10.1007/s12666-022-02848-3"
        },
        {
            number: 22,
            year: 2023,
            authors: "Anderson, N. J., Bin Zhang, A. C. Meng, Xiaoman Zhang, K. P. Lijesh, M. M. Khonsari, and W. J. Meng.",
            title: "Cr-Containing Diamond-Like Carbon Coatings Deposited on 316 Stainless Steel Substrates: Characterization and Interfacial Fracture-Toughness Measurements.",
            journal: "Surface and Coatings Technology 462 (2023): 129462.",
            doi: "https://doi.org/10.1016/j.surfcoat.2023.129462"
        },
        {
            number: 23,
            year: 2023,
            authors: "Amooie, Mohammad A., K. P. Lijesh, Ali Mahmoudi, Elaheh Azizian-Farsani, and Michael M. Khonsari.",
            title: "On the Characteristics of Fatigue Fracture with Rapid Frequency Change.",
            journal: "Entropy 25, no. 6 (2023): 840.",
            doi: "https://doi.org/10.3390/e25060840"
        },
        {
            number: 24,
            year: 2022,
            authors: "Shah, Raj, Lijesh K. P., Michael M. Khonsari, Anthony Schevon, and Shashank Bharadwaj.",
            title: "Design and Development of an Innovative Instrument to Measure Consistency and Useful Life in Greases.",
            journal: "Petro-Online (2022).",
            doi: null
        },
        {
            number: 25,
            year: 2021,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "A Unified Treatment of Tribo-Components Degradation Using Thermodynamics Framework: A Review on Adhesive Wear.",
            journal: "Entropy 23, no. 10 (2021): 1329.",
            doi: "https://doi.org/10.3390/e23101329"
        },
        {
            number: 26,
            year: 2021,
            authors: "Lijesh, K. P., M. M. Khonsari, Roger A. Miller, and Raj Shah.",
            title: "Evaluating Grease Degradation through Contact Angle Approach.",
            journal: "Lubricants 9, no. 1 (2021): 11.",
            doi: "https://doi.org/10.3390/lubricants9010011"
        },
        {
            number: 27,
            year: 2020,
            authors: "Lijesh, K. P., M. M. Khonsari, and Roger A. Miller.",
            title: "Assessment of Water Contamination on Grease Using the Contact Angle Approach.",
            journal: "Tribology Letters 68, no. 4 (2020): 103.",
            doi: "https://doi.org/10.1007/s11249-020-01339-0"
        },
        {
            number: 28,
            year: 2020,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "Characterization of Multiple Wear Mechanisms through Entropy.",
            journal: "Tribology International 152 (2020): 106548.",
            doi: "https://doi.org/10.1016/j.triboint.2020.106548"
        },
        {
            number: 29,
            year: 2020,
            authors: "Madhu, H. C., Vimal Edachery, K. P. Lijesh, Chandra Shekhar Perugu, and Satish V. Kailas.",
            title: "Fabrication of Wear-Resistant Ti₃AlC₂/Al₃Ti Hybrid Aluminum Composites by Friction Stir Processing.",
            journal: "Metallurgical and Materials Transactions A 51, no. 8 (2020): 4086–4099.",
            doi: "https://doi.org/10.1007/s11661-020-05821-1"
        },
        {
            number: 30,
            year: 2020,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "Characterization of Abrasive Wear Using Degradation Coefficient.",
            journal: "Wear 450–451 (2020): 203220.",
            doi: "https://doi.org/10.1016/j.wear.2020.203220"
        },
        {
            number: 31,
            year: 2019,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "Application of Thermodynamic Principles in Determining the Degradation of Tribo-Components Subjected to Oscillating Motion in Boundary and Mixed Lubrication Regimes.",
            journal: "Wear 436–437 (2019): 203002.",
            doi: "https://doi.org/10.1016/j.wear.2019.203002"
        },
        {
            number: 32,
            year: 2019,
            authors: "Lijesh, K. P., Mohammad Mehdizadeh, and Michael M. Khonsari.",
            title: "Online Monitoring of Metal Fatigue Life.",
            journal: "Structural Health Monitoring, first published online in 2019.",
            doi: "https://doi.org/10.1177/1475921719871668"
        },
        {
            number: 33,
            year: 2019,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "On the Degradation of Tribo-Components Undergoing Oscillating Sliding Contact.",
            journal: "Tribology International 135 (2019): 18–28.",
            doi: "https://doi.org/10.1016/j.triboint.2019.02.016"
        },
        {
            number: 34,
            year: 2019,
            authors: "Chaichi, Ardalan, Alisha Prasad, Lijesh K. P., Shahensha Shaik, Ali Hemmasian Ettefagh, Vinod Dasa, S. M. Guo, et al.",
            title: "Improvement of Tribological and Biocompatibility Properties of Orthopedic Materials Using Piezoelectric Direct Discharge Plasma Surface Modification.",
            journal: "ACS Biomaterials Science & Engineering 5 (2019): 2147–2159.",
            doi: "https://doi.org/10.1021/acsbiomaterials.9b00009"
        },
        {
            number: 35,
            year: 2019,
            authors: "Lijesh, K. P.",
            title: "Design Methodology for Monolithic-Layer Radial Passive Magnetic Bearing.",
            journal: "Proceedings of the Institution of Mechanical Engineers, Part J: Journal of Engineering Tribology 233, no. 6 (2019): 992–1000.",
            doi: "https://doi.org/10.1177/1350650118806372"
        },
        {
            number: 36,
            year: 2019,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "On the Assessment of Mechanical Degradation of Grease Using Entropy Generation Rate.",
            journal: "Tribology Letters 67, no. 2 (2019): 50.",
            doi: "https://doi.org/10.1007/s11249-019-1165-8"
        },
        {
            number: 37,
            year: 2019,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "On the Degradation of Tribo-Components in Boundary and Mixed Lubrication Regimes.",
            journal: "Tribology Letters 67, no. 1 (2019): 12.",
            doi: "https://doi.org/10.1007/s11249-018-1125-8"
        },
        {
            number: 38,
            year: 2019,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "On the Onset of Steady State during Transient Adhesive Wear.",
            journal: "Tribology International 130 (2019): 378–386.",
            doi: "https://doi.org/10.1016/j.triboint.2018.10.004"
        },
        {
            number: 39,
            year: 2018,
            authors: "Rajpal, Rohit, Lijesh K. P., and K. V. Gangadharan.",
            title: "Experimental Investigation of 3D-Printed Polymer-Based MR Sandwich Beam under Discretized Magnetic Field.",
            journal: "Journal of the Brazilian Society of Mechanical Sciences and Engineering 40, no. 12 (2018): 569.",
            doi: null
        },
        {
            number: 40,
            year: 2018,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "On the Useful Life of Tribo-Pairs Experiencing Variable Loading and Sliding Speed.",
            journal: "Wear 416–417 (2018): 103–114.",
            doi: "https://doi.org/10.1016/j.wear.2018.10.005"
        },
        {
            number: 41,
            year: 2018,
            authors: "Lijesh, K. P.",
            title: "Design Methodology for Monolithic-Layer Radial Passive Magnetic Bearing.",
            journal: "Proceedings of the Institution of Mechanical Engineers, Part J: Journal of Engineering Tribology, online publication (2018).",
            doi: "https://doi.org/10.1177/1350650118806372"
        },
        {
            number: 42,
            year: 2018,
            authors: "Lijesh, K. P., and M. M. Khonsari.",
            title: "On the Modeling of Adhesive Wear with Consideration of Loading Sequence.",
            journal: "Tribology Letters 66 (2018): 105.",
            doi: "https://doi.org/10.1007/s11249-018-1058-2"
        },
        {
            number: 43,
            year: 2018,
            authors: "Lijesh, K. P., M. M. Khonsari, and Satish V. Kailas.",
            title: "On the Integrated Degradation Coefficient for Adhesive Wear: A Thermodynamic Approach.",
            journal: "Wear 408–409 (2018): 138–150.",
            doi: "https://doi.org/10.1016/j.wear.2018.05.004"
        },
        {
            number: 44,
            year: 2018,
            authors: "Lijesh, K. P., Deepak Kumar, and K. V. Gangadharan.",
            title: "Design of Magneto-Rheological Brake for Optimum Dimension.",
            journal: "Journal of the Brazilian Society of Mechanical Sciences and Engineering 40, no. 3 (2018): 161.",
            doi: null
        },
        {
            number: 45,
            year: 2018,
            authors: "Rajpal, Rohit, Lijesh K. P., and K. V. Gangadharan.",
            title: "Parametric Studies on Bending Stiffness and Damping Ratio of Sandwich Structures.",
            journal: "Additive Manufacturing 22 (2018): 583–591.",
            doi: null
        },
        {
            number: 46,
            year: 2018,
            authors: "Kuriachen, Basil, Lijesh K. P., and P. Kuppan.",
            title: "Multi-Response Optimization and Experimental Investigations into the Impact of Wire EDM on the Tribological Properties of Ti-6Al-4V.",
            journal: "Transactions of the Indian Institute of Metals 71, no. 6 (2018): 1331–1341.",
            doi: null
        },
        {
            number: 47,
            year: 2018,
            authors: "Kumar, Deepak, K. B. Deepak, S. M. Muzakkir, M. F. Wani, and K. P. Lijesh.",
            title: "Enhancing Tribological Performance of Ti-6Al-4V by Sliding Process.",
            journal: "Tribology—Materials, Surfaces & Interfaces 12, no. 3 (2018): 1–7.",
            doi: null
        },
        {
            number: 48,
            year: 2018,
            authors: "Lijesh, K. P., Mrityunjay Doddamani, and S. I. Bekinal.",
            title: "A Pragmatic Optimization of Axial Stack-Radial Passive Magnetic Bearings.",
            journal: "Journal of Tribology 140, no. 2 (2018): 021901.",
            doi: null
        },
        {
            number: 49,
            year: 2018,
            authors: "Lijesh, K. P., Mrityunjay Doddamani, S. I. Bekinal, and S. M. Muzakkir.",
            title: "A Study on the Multi-Objective Optimization of Stacked Radial Passive Magnetic Bearing.",
            journal: "Proceedings of the Institution of Mechanical Engineers, Part J: Journal of Engineering Tribology 232, no. 9 (2018): 1140–1159.",
            doi: null
        },
        {
            number: 50,
            year: 2017,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "Design and Development of Permanent Magnet-Hydrodynamic Hybrid Journal Bearing.",
            journal: "Journal of Tribology 139, no. 4 (2017): 044501.",
            doi: null
        },
        {
            number: 51,
            year: 2017,
            authors: "Lijesh, K. P., Deepak Kumar, and Harish Hirani.",
            title: "Effect of Disc Hardness on MR Brake Performance.",
            journal: "Engineering Failure Analysis 74 (2017): 228–238.",
            doi: null
        },
        {
            number: 52,
            year: 2016,
            authors: "Lijesh, K. P., S. M. Muzakkir, and Harish Hirani.",
            title: "Control on Wear of Journal Bearing Operating in Mixed Lubrication Regime Using Grooving Arrangements.",
            journal: "Industrial Lubrication and Tribology 68, no. 4 (2016): 458–465.",
            doi: null
        },
        {
            number: 53,
            year: 2016,
            authors: "Muzakkir, S. M., Lijesh K. P., and Harish Hirani.",
            title: "Influence of Surfactants on Tribological Behaviors of MWCNT.",
            journal: "Tribology—Materials, Surfaces & Interfaces 10, no. 2 (2016): 74–81.",
            doi: null
        },
        {
            number: 54,
            year: 2016,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "Failure Mode and Effect Analysis of Active Magnetic Bearings.",
            journal: "Tribology in Industry 38, no. 1 (2016): 90–101.",
            doi: null
        },
        {
            number: 55,
            year: 2016,
            authors: "Lijesh, K. P., S. M. Muzakkir, and Harish Hirani.",
            title: "Rheological Measurement of Redispersibility and Settling to Analyze the Effect of Surfactants on MR Particles.",
            journal: "Tribology—Materials, Surfaces & Interfaces 10, no. 1 (2016): 53–62.",
            doi: null
        },
        {
            number: 56,
            year: 2016,
            authors: "Lijesh, K. P., S. M. Muzakkir, and Harish Hirani.",
            title: "Failure Mode and Effect Analysis of Passive Magnetic Bearing.",
            journal: "Engineering Failure Analysis 62 (2016): 1–20.",
            doi: null
        },
        {
            number: 57,
            year: 2015,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "Magnetic Bearing Using Rotation-Magnetized Direction Configuration.",
            journal: "Journal of Tribology 137, no. 4 (2015): 042201.",
            doi: null
        },
        {
            number: 58,
            year: 2015,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "Optimization of Eight-Pole Radial Active Magnetic Bearing.",
            journal: "Journal of Tribology 137, no. 2 (2015): 024502.",
            doi: null
        },
        {
            number: 59,
            year: 2015,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "Development of Analytical Equations for Design and Optimization of Axially Polarized Radial Passive Magnetic Bearing.",
            journal: "Journal of Tribology 137, no. 1 (2015): 011103.",
            doi: null
        },
        {
            number: 60,
            year: 2015,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "Design and Development of Halbach Electromagnet for Active Magnetic Bearing.",
            journal: "Progress in Electromagnetics Research C 56 (2015): 173–181.",
            doi: null
        },
        {
            number: 61,
            year: 2015,
            authors: "Lijesh, K. P., S. M. Muzakkir, and Harish Hirani.",
            title: "Experimental Tribological Performance Evaluation of Nanolubricant Using Multi-Walled Carbon Nanotubes.",
            journal: "International Journal of Applied Engineering Research 10, no. 6 (2015): 14543–14550.",
            doi: null
        },
        {
            number: 62,
            year: 2015,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "Probabilistic Design of Spur Gear.",
            journal: "International Journal of Current Engineering and Technology (2015).",
            doi: null
        },
        {
            number: 63,
            year: 2015,
            authors: "Lijesh, K. P., S. M. Muzakkir, and Harish Hirani.",
            title: "Failure Analysis of Rolling Contact Bearing for Flywheel Energy Storage Systems.",
            journal: "International Journal of Current Engineering and Technology 5, no. 1 (2015): 439–443.",
            doi: null
        },
        {
            number: 64,
            year: 2015,
            authors: "Muzakkir, S. M., Lijesh K. P., and Harish Hirani.",
            title: "Effect of Cylindricity on the Tribological Performance of Heavily Loaded Slow-Speed Journal Bearing.",
            journal: "Proceedings of the Institution of Mechanical Engineers, Part J: Journal of Engineering Tribology 229, no. 2 (2015): 178–195.",
            doi: null
        },
        {
            number: 65,
            year: 2015,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "The Performance of Hybrid Journal Bearing under Extreme Operating Conditions.",
            journal: "International Journal of Current Engineering and Technology 5, no. 1 (2015): 277–282.",
            doi: null
        },
        {
            number: 66,
            year: 2014,
            authors: "Muzakkir, S. M., Lijesh K. P., and Harish Hirani.",
            title: "Tribological Failure Analysis of a Heavily Loaded Slow-Speed Hybrid Journal Bearing.",
            journal: "Engineering Failure Analysis 40 (2014): 97–113.",
            doi: null
        },
        {
            number: 67,
            year: 2014,
            authors: "Akash, Kumar, K. P. Lijesh, Vedant Chittlangia, and Harish Hirani.",
            title: "Design and Implementation of Adaptive PID Controller for Active Magnetic Bearings.",
            journal: "Technology Letters 1, no. 12 (2014): 18–24.",
            doi: null
        },
        {
            number: 68,
            year: 2014,
            authors: "Lijesh, K. P., and Harish Hirani.",
            title: "Stiffness and Damping Coefficients for Rubber-Mounted Hybrid Bearing.",
            journal: "Lubrication Science 26, no. 5 (2014): 301–314.",
            doi: null
        }
    ];

    const publicationContainer =
        document.getElementById("publicationContainer");

    const searchInput =
        document.getElementById("publicationSearch");

    const yearFilter =
        document.getElementById("yearFilter");

    const resultsSummary =
        document.getElementById("resultsSummary");

    function createYearOptions() {
        const years = [
            ...new Set(
                publications.map(publication => publication.year)
            )
        ].sort((a, b) => b - a);

        years.forEach(year => {
            const option = document.createElement("option");
            option.value = year;
            option.textContent = year;
            yearFilter.appendChild(option);
        });
    }

    function createPublicationCard(publication) {
        const article = document.createElement("article");
        article.className = "publication-card";

        const number = document.createElement("div");
        number.className = "publication-number";
        number.textContent = publication.number;

        const content = document.createElement("div");

        const title = document.createElement("h3");
        title.className = "publication-title";
        title.textContent = publication.title;

        const authors = document.createElement("p");
        authors.className = "publication-authors";
        authors.textContent = publication.authors;

        const journal = document.createElement("p");
        journal.className = "publication-journal";
        journal.innerHTML = `<em>${publication.journal}</em>`;

        content.appendChild(title);
        content.appendChild(authors);
        content.appendChild(journal);

        /*
         * The journal link is created only when a DOI URL exists.
         * Nothing is displayed below publications that do not have a DOI.
         */
        if (publication.doi) {
            const journalLink = document.createElement("a");

            journalLink.className = "journal-link";
            journalLink.href = publication.doi;
            journalLink.target = "_blank";
            journalLink.rel = "noopener noreferrer";

            journalLink.textContent = "View on Journal Website";

            journalLink.setAttribute(
                "aria-label",
                `View ${publication.title} on the journal website`
            );

            content.appendChild(journalLink);
        }

        article.appendChild(number);
        article.appendChild(content);

        return article;
    }

    function renderPublications() {
        const searchTerm =
            searchInput.value.trim().toLowerCase();

        const selectedYear =
            yearFilter.value;

        const filteredPublications = publications.filter(publication => {
            const searchableText = [
                publication.number,
                publication.year,
                publication.authors,
                publication.title,
                publication.journal
            ]
                .join(" ")
                .toLowerCase();

            const matchesSearch =
                searchableText.includes(searchTerm);

            const matchesYear =
                selectedYear === "all" ||
                publication.year.toString() === selectedYear;

            return matchesSearch && matchesYear;
        });

        publicationContainer.innerHTML = "";

        resultsSummary.textContent =
            `${filteredPublications.length} publication${
                filteredPublications.length === 1 ? "" : "s"
            } displayed`;

        if (filteredPublications.length === 0) {
            const emptyState = document.createElement("div");
            emptyState.className = "empty-state";
            emptyState.textContent =
                "No publications match the selected search criteria.";

            publicationContainer.appendChild(emptyState);
            return;
        }

        const groupedPublications = filteredPublications.reduce(
            (groups, publication) => {
                if (!groups[publication.year]) {
                    groups[publication.year] = [];
                }

                groups[publication.year].push(publication);
                return groups;
            },
            {}
        );

        Object.keys(groupedPublications)
            .sort((a, b) => Number(b) - Number(a))
            .forEach(year => {
                const yearSection =
                    document.createElement("section");

                yearSection.className = "year-group";

                const heading =
                    document.createElement("h3");

                heading.className = "year-heading";
                heading.textContent = year;

                const list =
                    document.createElement("div");

                list.className = "publication-list";

                groupedPublications[year].forEach(publication => {
                    list.appendChild(
                        createPublicationCard(publication)
                    );
                });

                yearSection.appendChild(heading);
                yearSection.appendChild(list);

                publicationContainer.appendChild(yearSection);
            });
    }

    searchInput.addEventListener(
        "input",
        renderPublications
    );

    yearFilter.addEventListener(
        "change",
        renderPublications
    );

    document.getElementById("currentYear").textContent =
        new Date().getFullYear();

    createYearOptions();
    renderPublications();
</script>

</body>
</html>
