# Advanced-cctv-analysis

// Criminal Detection System - CCTV + Face Matching (Simulated in C)
// Note: Real DeepFace runs in Python. This is a simulation for academic/demo purposes.
***************************************************************************************************************************************************
#include <stdio.h>
#include <string.h>
#include <time.h>
void send_alert_to_cloud(const char *criminal_name, const char *location) {
time_t now;
time(&now);
printf("ALERT SENT\n");
printf("Criminal: %s\n", criminal_name);
printf("Location: %s\n", location);
printf("Time: %s\n", ctime(&now));
}
// Simulate facial recognition result
int detect_criminal_face(const char *captured_face, const char *db_face) { return strcmp(captured_face, db_face) == 0;
}
int main() {
// Simulated face capture from CCTV char captured_face[100] = "face123.jpg";
// Simulated criminal database
char known_faces [] [100] = {
// Match
"face101.jpg",
"face122.jpg",
"face123.jpg",
"face134.jpg"
};
int num_faces = sizeof(known_faces) / sizeof(known_faces[0]); int match found = 0;
for(int i = 0; i < num faces; i++) {
if(detect_criminal_face(captured_face, known_faces[i])) { printf("MATCH FOUND: %s\n", known_faces[i]); send_alert_to_cloud(known_faces[i], "Gate A"); match_found = 1; break:
}

if(!match found) { printf("No match found.\n");

return 0:
