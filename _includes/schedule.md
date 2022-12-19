
## Current Schedule

<div>
    <table>
        <thead>
            <th>Day</th>
            <th>Time</th>
            <th>Location</th>
            <th>Type</th>
            <th>Distance</th>
        </thead>
        <tbody>
            {% for item in site.data.schedule %}
            <tr>
                <td>{{item.day}}</td>
                <td>{{item.time}}</td>
                <td><a href="{{item.location_link}}">{{item.location}}</a></td>
                <td>{{item.type}}</td>
                <td>{{item.distance}}</td>
            </tr>
            <!-- |{{item.day}}|{{item.time}}|[{{item.location}}]({{item.loction_link}})|{{item.type}}|{{item.distance}}| -->
            {% endfor %}
        </tbody>
    </table>
</div>

<!-- |Day| Time | Location | Type | Distance | -->
<!-- |---|------|----------|------|----------| -->
