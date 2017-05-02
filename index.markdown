---
layout: index
published: true
extra_js:
 - https://learningcircles.p2pu.org/en/studygroups/?course_id=2&callback=renderCircles
---

## Take the course in person

Learning Circles offer the opportunity to work through the course with your local community. Join a Learning Circle near you below, or create your own!

<div id="lc-container" class="row">
<div class="col-md-4">{% include lc-card.html %}</div>
</div>

Or <a href="https://learningcircles.p2pu.org/" class="btn btn-primary">create your own</a>

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
        if (circle.image_url.length > 0){
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

## Goals of this Course 
The goal of this course is for participants to use our framework to assist in the design and/or implementation of a makerspace or maker program that supports learning in a museum or library. The course can support people who are beginning the development of a new makerspace or maker program or improving upon one that is already up and running. 

### Intended Audience
This course is intended for museum and library professionals, or anybody who is designing a makerspace. We encourage participants to engage in the sessions with team members, from your own organization and/or with partner organizations. 

### Format
The course consists of a 30 minute reading and four two-hour sessions, each of which will take about two hours to work through. The course has been designed to be taken as a learning circle: a model of peer-facilitated learning that is designed to add face-to-face interaction and social accountability to the online course experience. After each session, participants are encouraged to share their work on the virtual forum: writing comments, sharing a photo, or uploading a video. If you'd rather go through the course on your own, go right ahead! There are no log ins or sign ups required.

This is an open course, meaning that there is no registration or logging in required to access any  of the materials. All course materials are licensed under a [CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/), and were developed with the support of [Peer 2 Peer University](https://www.p2pu.org/).


