# Intelligent Medical Receptionist System

## Technology Stack
- **Frontend**: React.js with TypeScript
- **Backend**: n8n Workflow Automation
- **Database**: PostgreSQL (Supabase)
- **AI**: OpenAI GPT Models
- **Calendar Integration**: Google Calendar API

## Overview

This Intelligent Medical Receptionist System provides a comprehensive solution for healthcare facilities to automate patient interactions and appointment management. The system features an advanced conversational AI interface that enables patients to schedule, modify, and manage appointments using natural language processing. It integrates seamlessly with existing clinic management systems and calendar platforms to streamline administrative workflows.

## Application Interface

The system features a modern, user-friendly chat interface that enables natural conversation between patients and the AI receptionist. The responsive design ensures optimal experience across all devices, from desktop computers to mobile phones.

**Key Interface Features:**
- Real-time chat with typing indicators
- Session persistence and conversation history
- Mobile-responsive layout
- Accessibility-compliant design
- Multi-language support capabilities

## System Architecture

The application consists of two main components:

### Frontend (React)
- Conversational chat interface
- Real-time communication with backend
- Responsive design for all devices
- Session management and chat history

### Backend (n8n)
- AI-powered request processing
- Multi-service orchestration
- Database and calendar integration
- Webhook-based API

**Backend Architecture:**
The n8n-based backend provides a robust workflow engine that orchestrates various services and APIs. The architecture supports scalable processing of patient requests while maintaining data security and compliance standards.

## Core Features

### For Patients
- **Natural Conversation**: Communicate in plain language, no forms required
- **Appointment Booking**: Schedule appointments with preferred dates and times
- **Appointment Management**: Reschedule or cancel existing appointments
- **Availability Checking**: View available time slots
- **Patient Registration**: Register as a new patient through conversation
- **24/7 Availability**: Access the system anytime

### For Clinic Staff
- **Automated Scheduling**: Reduces administrative workload
- **Calendar Integration**: Syncs with existing calendar systems
- **Patient Database**: Automatic record management
- **Conversation History**: Full audit trail of interactions
- **Consistent Service**: Standardized responses and procedures

## Technical Architecture

### Frontend Stack
- **Framework**: React
- **Communication**: REST API (Webhook)
- **State Management**: React Hooks
- **Styling**: Modern, responsive design

### Backend Stack
- **Workflow Engine**: n8n
- **AI Model**: OpenAI Chat Model
- **Database**: PostgreSQL
- **Integration**: Google Calendar / Calendar APIs
- **API**: Webhook-based endpoints

## How It Works

1. **Patient Interaction**: User sends a message through the chat interface
2. **Request Processing**: Frontend sends request to n8n webhook
3. **AI Analysis**: OpenAI model processes the request and determines intent
4. **Action Execution**: System performs necessary operations:
   - Search/create/update appointments
   - Manage calendar events
   - Handle patient records
5. **Context Management**: Conversation stored in PostgreSQL for continuity
6. **Response Generation**: AI formulates natural language response
7. **Response Delivery**: Answer displayed in chat interface

## Use Cases

### Booking Appointments
> **Patient**: "I'd like to schedule an appointment for next Tuesday at 2pm"  
> **AI**: "I'd be happy to help you schedule an appointment. Let me check availability for Tuesday at 2pm..."

### Rescheduling
> **Patient**: "Can I move my appointment to Thursday instead?"  
> **AI**: "Of course! Let me reschedule your appointment to Thursday..."

### New Patient Registration
> **Patient**: "I'm a new patient and would like to register"  
> **AI**: "Welcome! I'll help you register. May I have your full name to get started?"

### Checking Availability
> **Patient**: "What times are available this week?"  
> **AI**: "Here are the available time slots for this week..."

## Benefits

### Efficiency
- Significantly reduces incoming phone calls and inquiries
- Automates the complete appointment scheduling workflow
- Minimizes manual data entry and administrative tasks

### Patient Experience
- Immediate AI-powered responses without waiting
- Round-the-clock availability for scheduling needs
- Intuitive, human-like conversation flow
- Support for multiple languages and accessibility needs

### Operational Excellence
- Consistent service quality
- Reduced scheduling errors
- Complete conversation logs
- Scalable to handle growth

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- n8n instance
- PostgreSQL database
- OpenAI API key
- Calendar integration (Google Calendar, etc.)

### Installation

#### Frontend Setup
```bash
cd frontend
npm install
cp .env.example .env
# Configure REACT_APP_WEBHOOK_URL
npm start
```

#### Backend Setup
1. Import the n8n workflow from `/backend/workflow.json`
2. Configure credentials:
   - OpenAI API
   - PostgreSQL connection
   - Calendar integration
3. Set up webhook endpoints
4. Activate the workflow

### Environment Variables

#### Frontend (.env)
```env
VITE_CHATBOT_WEBHOOK_URL=https://webhook.....
```

#### Backend (n8n)
- OpenAI API Key
- PostgreSQL (supabase) connection string
- Calendar API credentials




## Security & Privacy

- All patient data is encrypted in transit and at rest
- HIPAA compliance considerations built-in
- Secure webhook authentication
- Session management and timeout policies
- Audit logging for all interactions

## Future Enhancements

- [ ] SMS/WhatsApp integration
- [ ] Insurance verification
- [ ] Prescription refill requests
- [ ] Lab results notifications
- [ ] Video consultation scheduling



## License



---

**Intelligent Medical Receptionist** - Revolutionizing healthcare administration through AI-powered automation
