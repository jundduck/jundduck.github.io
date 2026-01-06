---
layout: post
title: A1 Autonomous Car Challenge 
inline: true
---



{%- comment -%}
cid: 이 항목만의 고유 접두사. page.slug가 있으면 사용하고, 없으면 title을 slugify 해서 사용.
모든 collapse의 id / href를 이 cid로 네임스페이스화해서 충돌 방지.
{%- endcomment -%}
{% assign cid = page.slug | default: page.title | slugify %}

<style>
  /* 버튼 간격/스타일 */
  .competition-entry .links{ display:flex; flex-wrap:wrap; }
  .competition-entry .links a.btn{
    color:var(--global-text-color);
    border:1px solid var(--global-text-color);
    padding:0.25rem 1rem;
    margin-right:1rem;
    margin-bottom:0.5rem;
  }
  .competition-entry .links a.btn:hover{
    color:var(--global-theme-color);
    border-color:var(--global-theme-color);
    text-decoration:none;
  }

  /* collapse 컨테이너에서 잔선 제거 + 펼쳐질 때만 테두리/패딩 */
  .collapse, .collapsing{
    overflow:hidden;
    box-sizing:border-box;
    transition:none !important;           /* 즉시 표시로 바꾸고 싶으면 이 값 유지 */
    /* transition: height 0.06s ease-out !important; */ /* 아주 빠른 애니메이션 원하면 이 줄을 쓰고 위 줄 주석 */
  }
  .collapse{ border:0; padding:0; margin-top:0 !important; }
  .collapsing, .collapse.show{
    border:1px dashed var(--global-text-color);
    border-radius:6px;
    padding:12px;
    margin-top:0.5rem;
  }

  .toggle-panel{ border:0; padding:0; margin:0; }
</style>

<div class="competition-entry">
  <div class="row no-gutters align-items-start">
    <!-- 왼쪽: 이미지 -->
    <div class="col-md-4 col-12 mb-3 mb-md-0">
      <img src="{{ '/assets/img/A1.jpg' | relative_url }}"
           alt="QRC Korea"
           class="img-fluid rounded z-depth-1"
           style="max-width:260px;">
    </div>

    <!-- 오른쪽: 텍스트 -->
    <div class="col-md-8 col-12 pl-md-3">
      <div class="font-weight-bold mb-1">
        A1 Autonomous Car Challenge — <em>On going</em>
      </div>

      <!-- Team Member -->
      <div class="text"><strong>Participants:</strong> Junseok Lee, Hyeonseo Oh, Woongje Jo, SeoJin Yoo, JooWon Kim </div>

      <!-- Host -->
      <div class="text-muted">Ministry of Trade, Industry and Resources, KIAPI, MORAI</div>


      <!-- Brief Explanation -->
      <p class="mt-2 mb-1">
        End to End Autonmous Driving Racing(MORAI Sim) & Real Car Racing (Yongin Speedway).
      </p>




      <!-- 각 버튼들 따로 움직임
      <div class="links mt-3">
        <a class="btn btn-sm z-depth-0" data-toggle="collapse"
           href="#{{ cid }}-team"
           role="button" aria-expanded="false" aria-controls="{{ cid }}-team">Team</a>

        <a class="btn btn-sm z-depth-0" data-toggle="collapse"
           href="#{{ cid }}-host"
           role="button" aria-expanded="false" aria-controls="{{ cid }}-host">Host</a>

        <a class="btn btn-sm z-depth-0" data-toggle="collapse"
           href="#{{ cid }}-award"
           role="button" aria-expanded="false" aria-controls="{{ cid }}-award">Award</a>

        <a href="https://example.com/qrc-korea" target="_blank" rel="noopener noreferrer"
           class="btn btn-sm z-depth-0">Project Page</a>
      </div>



      <!-- 버튼들 -->
      <div id="{{ cid }}-team" class="collapse" aria-labelledby="btn-{{ cid }}-team">
        <div class="toggle-panel">
          <strong>Team Members</strong><br/>
          Junseok Lee, Teammate A, Teammate B
        </div>
      </div>

      <div id="{{ cid }}-host" class="collapse" aria-labelledby="btn-{{ cid }}-host">
        <div class="toggle-panel">
          <strong>Organizer</strong><br/>
          Korea Robotics Aircraft Competition (KRAC)
        </div>
      </div>

      <div id="{{ cid }}-award" class="collapse" aria-labelledby="btn-{{ cid }}-award">
        <div class="toggle-panel">
          <strong>Result</strong><br/>
          <em>3rd Place</em> — Final ranking among <b>51 teams</b>. 
        </div>
      </div>


    </div>
  </div>
</div>
