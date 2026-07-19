---
layout: page
title: About
permalink: /
nav: true
nav_order: 1
description: "Academic website of Dr. Lijesh Koottaparambil"
---

<style>
  /* Custom homepage container */
  .custom-home {
    display: grid;
    grid-template-columns: 230px minmax(360px, 1fr) 300px;
    gap: 30px;
    align-items: start;
    width: 100%;
    margin-top: 20px;
  }

  /* Purple profile sidebar */
  .home-sidebar {
    min-height: 650px;
    overflow: hidden;
    background: #461d7c;
    border: 1px solid #35145f;
  }

  .home-profile-image {
    display: block;
    width: 100%;
    height: auto;
    margin: 0;
    object-fit: cover;
  }

  .home-stats {
    padding: 24px 20px;
  }

  .stat-item {
    margin-bottom: 24px;
  }

  .stat-number {
    display: block;
    color: #fdd023;
    font-size: 28px;
    font-weight: 700;
    line-height: 1.1;
  }

  .stat-label {
    display: block;
    margin-top: 5px;
    color: #ffffff;
    font-size: 15px;
  }

  /* Main biography section */
  .home-main {
    min-width: 0;
    padding-top: 4px;
  }

  .home-header {
    margin-bottom: 35px;
    padding-bottom: 12px;
    border-bottom: 2px solid #461d7c;
  }

  .home-header h1 {
    margin: 0;
    font-size: 34px;
    font-weight: 400;
    line-height: 1.2;
  }

  .home-position {
    margin: 8px 0 0;
    font-size: 14px;
    line-height: 1.5;
  }

  .home-biography {
    font-size: 16px;
    line-height: 1.65;
  }

  .home-biography p {
    margin-bottom: 22px;
  }

  /* Research-interest pills */
  .research-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 9px;
    margin-top: 25px;
  }

  .research-tags span {
    display: inline-block;
    padding: 7px 12px;
    border: 1px solid #461d7c;
    border-radius: 20px;
    font-size: 13px;
    line-height: 1.2;
  }

  /* Professional links */
  .home-social-links {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 30px;
  }

  .home-social-links a {
    display: inline-block;
    padding: 9px 14px;
    border-radius: 4px;
    background: #461d7c;
    color: #ffffff !important;
    font-size: 14px;
    font-weight: 500;
    text-decoration: none !important;
  }

  .home-social-links a:hover {
    background: #5f2d91;
    color: #fdd023 !important;
  }

  /* News panel */
  .home-news {
    padding: 22px;
    background: #f3f3f3;
    border-top: 6px solid #461d7c;
  }

  .home-news h2 {
    margin: 0 0 22px;
    font-size: 24px;
    font-weight: 500;
  }

  .news-item {
    margin-bottom: 18px;
    padding-bottom: 16px;
    border-bottom: 1px solid #d6d6d6;
  }

  .news-year {
    display: block;
    margin-bottom: 5px;
    color: #461d7c;
    font-size: 13px;
    font-weight: 700;
  }

  .news-item p {
    margin: 0;
    font-size: 14px;
    line-height: 1.5;
  }

  .news-link {
    display: inline-block;
    margin-top: 5px;
    font-weight: 600;
  }


  /* Tablet layout */
  @media screen and (max-width: 1100px) {
    .custom-home {
      grid-template-columns: 210px minmax(0, 1fr);
    }

    .home-news {
      grid-column: 1 / -1;
    }
  }

  /* Mobile layout */
  @media screen and (max-width: 700px) {
    .custom-home {
      display: block;
    }

    .home-sidebar {
      min-height: auto;
      margin-bottom: 28px;
    }

    .home-profile-image {
      max-height: 430px;
      object-position: top;
    }

    .home-main {
      margin-bottom: 30px;
    }

    .home-header h1 {
      font-size: 29px;
    }

    .home-news {
      margin-top: 25px;
    }
  }
</style>
