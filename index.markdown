---
layout: index
published: true
extra_js:
 - https://learningcircles.p2pu.org/en/studygroups/?course_id=176&callback=renderCircles
---

### Course Goal
The goal of this course is to assist in the design and/or implementation of a makerspace or maker program that supports learning in a museum or library. The course can support people who are beginning the development of a new makerspace or maker program or be used to improve upon one that is already up and running.

### Intended Audience
This course is intended for museum and library professionals, or anybody who is designing a makerspace. We encourage participants to engage in the sessions with team members, from your own organization and/or with partner organizations. 

### Course Format: Learning Circles
The course consists of 30 minutes of background reading (Session Zero), and four two-hour sessions. While you can access the materials on your own, the course is designed to be taken as a learning circle: a model of peer-facilitated learning that is designed to add face-to-face interaction and social accountability to the online course experience. Learning circles offer the opportunity to work through this course with your colleagues or neighbors. After each session, participants are encouraged to share their work on the virtual forum with others who are taking the course. 

By creating a learning circle, you'll benefit from resources and a community that help you facilitate a peer discussion, as well as software tools that generate promotional materials and automatically remind participants of upcoming meetings. If you don't see a nearby learning circle on this page, you can create your own below - just be sure to select "Making and Learning" from the list of courses.
 
<p id="homepage-lc-button"><a href="https://learningcircles.p2pu.org/" class="btn btn-primary" id="lc-button">Create a new learning circle</a></p>

<div id="lc-container" class="row">
    <div class="col-md-4">{% include lc-card.html %}</div>
</div>



<script type="text/javascript">
    function renderCircle(circle, template) {
        var html = template.clone();
        html.find('.d-course_title').text(circle.course_title);
        html.find('.d-facilitator').text(circle.facilitator);
        html.find('.d-venue').text(circle.venue);
        html.find('.d-venue_address').text(circle.venue_address);
        html.find('.d-day').text(circle.day + 's');
        html.find('.d-start_date').text(circle.start_date);
        html.find('.d-meeting_time').text(circle.meeting_time); // format time here
        html.find('.d-time_zone').text(circle.time_zone);
        html.find('.d-end_time').text(circle.end_time);
        html.find('.d-weeks').text(circle.weeks);
        html.find('.d-url').attr('href', circle.url);
        if (circle.image_url && circle.image_url.length > 0){
            html.find('.d-image_url').attr('src', circle.image_url);
        }
        return html;
    }

    function renderCircles(circles){
        var container = $('#lc-container');
        var template = $(container.children()[0]).clone();
        container.children().remove();
        for (var i = 0; i< circles.length; ++i){
            var lcHtml = renderCircle(circles[i], template);
            container.append(lcHtml);
        }
    }
</script>
