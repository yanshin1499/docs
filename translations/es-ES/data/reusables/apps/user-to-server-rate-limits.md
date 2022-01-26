{% ifversion ghes %}By default, user-to-server{% else %}User-to-server{% endif %} requests are limited to {% ifversion ghae %}15,000{% elsif fpt or ghec or ghes %}5,000{% endif %} requests per hour and per authenticated user. All requests from OAuth applications authorized by a user or a personal access token owned by the user, and requests authenticated with any of the user's authentication credentials, share the same quota of {% ifversion ghae %}15,000{% elsif fpt or ghec or ghes %}5,000{% endif %} requests per hour for that user.